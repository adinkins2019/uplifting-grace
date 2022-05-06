<script>
    let name;
    let email;
    let message;
    function handleSubmit(event){
        event.preventDefault();
    }
</script>

<form on:submit={handleSubmit}> 
       <div><label for="name">Name: </label>
            <input type="text" name="name" id="name" class="contact-content">
        </div>
        <div>
            <label for="email">Email: </label>
            <input type="email" name="email" id="email" class="contact-content">
        </div>
        <div>
            <label for="message">Message: </label>
            <textarea name="message" id="message" cols="30" rows="10" class="contact-content"></textarea>
        </div>
        <div id="form-buttons">
            <button type="submit">Send</button>
            <button type="reset">Clear</button>
        </div>    
</form>
    
<style>
  .contact-content {
      padding: 2%;
      margin-left: 20px;
      width: 75%;
  }
  div {
      display: flex;
  }
  #name, #email {
      margin-left: 50px;
  }
  #form-buttons{
      display: flex;
      justify-content: center;
  }
  #form-buttons button{
      padding: 2%;
      margin: 1%;
      font-weight: 600;
      border-radius: 7%;
      color: #D0E1D4;
      background: #71697A;
      border: 2px solid #71697A
  }

  #form-buttons button:hover {
      color: #71697A;
      background: #D0E1D4;
      transition-duration: 0,5s;
      transform: scale(1.1);
  }
</style>