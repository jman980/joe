<!DOCTYPE html>
<html>
<head>
<style>
  body {
    background: linear-gradient(135deg, #000000, #1a0000, #330000);
    font-family: Arial, sans-serif;
    color: #ff1a1a;
    display: flex;
    justify-content: center;
    padding: 50px;
    margin: 0;
    min-height: 100vh;
  }

  form {
    background: linear-gradient(145deg, #330000, #ff0000, #ff1a1a);
    padding: 30px;
    border-radius: 20px;
    width: 400px;
    box-shadow: 0 0 25px #ff1a1a, 0 0 50px #ff0000 inset;
  }

  h2 {
    text-align: center;
    color: #ff1a1a;
    margin-bottom: 20px;
    text-shadow: 0 0 8px #ff0000;
  }

  label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
    color: #ff4d4d;
  }

  .field {
    margin-bottom: 15px;
  }

  input[type="text"], input[type="number"] {
    width: 100%;
    padding: 8px;
    border-radius: 8px;
    border: 2px solid #ff0000;
    background-color: #1a0000;
    color: #ff1a1a;
  }

  input[type="checkbox"] {
    margin-right: 10px;
    accent-color: #ff1a1a;
  }

  input[type="submit"] {
    width: 50%;
    padding: 6px;
    border-radius: 10px;
    border: none;
    background: linear-gradient(90deg, #ff1a1a, #ff0000, #990000);
    color: #ff1a1a;
    font-size: 14px;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 0 0 10px #ff1a1a, 0 0 20px #ff0000 inset;
    transition: all 0.3s ease;
    display: block;
    margin: 20px auto 0;
  }

  input[type="submit"]:hover {
    background: linear-gradient(90deg, #ff0000, #ff1a1a, #660000);
    box-shadow: 0 0 15px #ff4d4d, 0 0 30px #ff0000 inset;
  }

  #total {
    font-size: 20px;
    color: #ff1a1a;
    text-shadow: 0 0 5px #ff0000;
  }

  div > label {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 5px;
    background-color: #660000;
    padding: 5px 10px;
    border-radius: 8px;
    box-shadow: 0 0 8px #ff1a1a inset;
  }

  .quantity {
    width: 50px;
    margin-left: 10px;
    text-align: center;
    background-color: #1a0000;
    color: #ff1a1a;
    border: 2px solid #ff0000;
    border-radius: 5px;
  }
</style>
</head>

<body>

<form id="form">
  <h2>Joe's Sushi Order</h2>

  <div class="field">
    <label for="name">Name</label>
    <input type="text" name="name" id="name" required>
  </div>

  <div class="field">
    <label>Select Your Sushi:</label>
    <div>
      <label><input type="checkbox" name="food" value="Salad Basket" data-price="5"> Salad Basket<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Caviar" data-price="10"> Caviar<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Wasabi" data-price="2"> Wasabi<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Warm Trio Combo (Three Rolls)" data-price="15"> Warm Trio Combo<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Soy Sauce" data-price="1"> Soy Sauce<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Christmas Roll" data-price="12"> Christmas Roll<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Breakfast Sushi Roll" data-price="10"> Breakfast Sushi Roll<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Pink Monster Roll" data-price="13"> Pink Monster Roll<input type="number" min="1" value="1" class="quantity"></label>
      <label><input type="checkbox" name="food" value="Green Monster Roll" data-price="13"> Green Monster Roll<input type="number" min="1" value="1" class="quantity"></label>
    </div>
  </div>

  <div>
    <strong>Total: <span id="total">0</span></strong>
  </div>

  <input type="submit" id="button" value="Send Email">
</form>

<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
<script>
  emailjs.init('h8uXW8FrDGOuL6WjC');

  const form = document.getElementById('form');
  const totalSpan = document.getElementById('total');
  const checkboxes = form.querySelectorAll('input[type="checkbox"]');

  function calculateTotal() {
    let total = 0;
    checkboxes.forEach(cb => {
      if (cb.checked) {
        const price = parseFloat(cb.dataset.price);
        const qty = parseInt(cb.nextElementSibling.value);
        total += price * qty;
      }
    });
    totalSpan.textContent = total; // no $
  }

  checkboxes.forEach(cb => {
    cb.addEventListener('change', calculateTotal);
    cb.nextElementSibling.addEventListener('input', calculateTotal);
  });

  form.addEventListener('submit', function(event) {
    event.preventDefault();

    let orderDetails = '';
    checkboxes.forEach(cb => {
      if (cb.checked) {
        const qty = parseInt(cb.nextElementSibling.value);
        orderDetails += `${cb.value} x${qty}\n`;
      }
    });

    const totalInput = document.createElement('input');
    totalInput.type = 'hidden';
    totalInput.name = 'total';
    totalInput.value = totalSpan.textContent;
    form.appendChild(totalInput);

    emailjs.sendForm('jason78800', "Joe's Sushi", form)
      .then(() => {
        alert('Order sent!');
        form.reset();
        totalSpan.textContent = '0';
      }, (error) => {
        console.error('FAILED...', error);
        alert('Failed to send.');
      });
  });
</script>

</body>
</html>
