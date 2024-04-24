<template>
    <div class="contact-us-container">
      <h1>Welcome to Strathmore University</h1>
      <div class="contact-info">
        <p>If you have any questions or need assistance, feel free to reach out to us. We're here to help!</p>
        <div class="info-group">
          <label>Address:</label>
          <p class="info">Strathmore University, Ole Sangale Road, Madaraka, Nairobi, Kenya</p>
        </div>
        <div class="info-group">
          <label>Email:</label>
          <p class="info">info@strathmore.edu</p>
        </div>
        <div class="info-group">
          <label>Phone:</label>
          <p class="info">+254 (0)703-034000 / +254 (0)703-034200</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ContactUs',
  };
  </script>
  
  <style scoped>
  .contact-us-container {
    max-width: 600px;
    margin: 40px auto;
    padding: 20px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    text-align: center;
    background-color: #f9f9f9;
  }
  
  h1 {
    color: #007bff;
  }
  
  .contact-info > p {
    margin-bottom: 1.5rem;
  }
  
  .info-group {
    margin-bottom: 1.5rem;
  }
  
  .info-group label {
    font-weight: bold;
    color: #333;
  }
  
  .info {
    margin: 0;
    padding-left: 1rem;
    color: #555;
  }
  
  /* Add some decorative styling */
  .contact-us-container:before {
    content: '';
    display: block;
    width: 100%;
    height: 1px;
    background-color: #ddd;
    margin: 20px 0;
  }
  
  .info-group:after {
    content: '';
    display: block;
    width: 100%;
    height: 1px;
    background-color: #ddd;
    margin-top: 10px;
  }
  </style>
  