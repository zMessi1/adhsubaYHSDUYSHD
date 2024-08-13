document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    if (name === '' || email === '' || message === '') {
        alert('Por favor, completa todos los campos.');
    } else {
        alert(`Gracias por contactarnos, ${name}. Hemos recibido tu mensaje.`);
        document.getElementById('contact-form').reset();
    }
});
