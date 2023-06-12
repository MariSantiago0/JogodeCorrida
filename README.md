# Jogo de Corrida
<p> LINK-> https://drive.google.com/drive/folders/1Zi0ylGFRzeevQxhpdqevYwZSo09Woefb</p>

# Descrevendo
<p> 
  O intuito do jogo é o movimento do carro. Um jogo de corrida. Ao fazer o jogo foi necessário escolher uma cena do store assets de uma pista e um carro, além de utilizar 6 gameobjects específicos de cada cena. Após a escolha, realizei o objetivo do jogo, o movimento do carro. Adicionei um código ao carro que descreve o seu movimento.<br>
  Que foi: <br>
  
    public class CarMovement : MonoBehaviour  { 
  
    public float speed = 300f; // Aumente esse valor para aumentar a velocidade do carro 
    public float rotationSpeed = 100f; 

    private void Update()
    {
        float moveInput = Input.GetAxis("Vertical");
        float rotateInput = Input.GetAxis("Horizontal");

        // Movimento para frente e para trás
        transform.Translate(Vector3.forward * moveInput * speed * Time.deltaTime);

        // Rotação do carro
        transform.Rotate(Vector3.up * rotateInput * rotationSpeed * Time.deltaTime);
    }}

</p>
