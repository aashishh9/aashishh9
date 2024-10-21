<style>
  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  @keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
  }

  .gif-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
    width: 300px;
    margin: 0 auto;
    position: relative;
  }

  .gif-container img {
    border-radius: 50%; /* Makes it circular */
    animation: spin 4s linear infinite; /* Rotates continuously */
    width: 100%; 
    height: 100%;
  }

  .name-text {
    position: absolute;
    opacity: 0;
    animation: fadeIn 2s ease-in-out 4s forwards; /* Fades in after 4s */
    font-size: 24px;
    font-weight: bold;
    color: #333;
  }
</style>

<div class="gif-container">
  <img src="https://media.giphy.com/media/L3Vca26EaTIEU/giphy.gif" alt="Rotating GIF">
  <div class="name-text">Ashish Pawar</div>
</div>
