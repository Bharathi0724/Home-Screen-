document.getElementById('loginForm').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;
    const errorMessage = document.getElementById('errorMessage');

    // Simple client-side validation (for demo purposes only)
    if (username === 'admin' && password === 'admin123') {
        alert('Login successful!');
        errorMessage.style.display = 'none';
        // You can redirect to another page or perform other actions here
    } else {
        errorMessage.textContent = 'Invalid username or password';
        errorMessage.style.display = 'block';
    }
});
