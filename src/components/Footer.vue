<template>
  <div class="footer">
      <div class="contatos">
          <h3>Contatos</h3>
           <a href="tel:+55 21 989020276"><i class="fas fa-phone-square"></i></a>
           <a href="mailto:diogon21@yahoo.com.br"><i class="fas fa-envelope-square"></i></a>
           <a href="https://github.com/Diogonsc"><i class="fab fa-github-square"></i></a>
           <a href="https://www.linkedin.com/in/diogo-nascimento-02199879/"><i class="fab fa-linkedin"></i></a>
      </div>
  </div>
</template>

<script>
export default {

} 
</script>

<style >
h3{
    color: #006d77;
    text-align: center;
}
    .footer{
        width:100%;
        display: flex;
        align-items: center;
        justify-content: center;
    }
     .contatos a {
        color: #006d77;
        align-items: center;
        padding: 5px;
        text-decoration: none;
    }
    i{
        font-size: 20px;
    }
</style>