# Jupyter Notebook with Docker

## 🚀 Installation

1. **Build the Docker Image**

   ```sh
   docker build -t my-jupyter-image .
   ```

2. **Run the Jupyter Container**

   ```sh
   docker run -d --name jupyter-container -p 8888:8888 my-jupyter-image
   ```

3. **Access Jupyter Notebook**
   In VSCode, select a new kernel (existing jupyter server) and paste this address:
   ```
   http://localhost:8888/lab?token=c8a36a576782b16bb08877ae120d419186518e2d3ce822df
   ```
4. **Token Issue?**
   If the token is invalid, find the correct one with:
   ```sh
   docker logs jupyter-container
   ```

📌 Your Jupyter notebooks will now be accessible in VS Code or your browser!
