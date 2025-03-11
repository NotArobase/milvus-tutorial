# Use this tutorial with Docker

## 🚀 Installation

1. **Build the Docker Image**

   ```sh
   docker build -t my-jupyter-image .
   ```

2. **Run the Jupyter Container**

   ```sh
   docker run -d --name jupyter-container -p 8888:8888 my-jupyter-image
   ```

3. **Look for the server URL**
   Find the server app URL in the logs:

   ```sh
   docker logs jupyter-container
   ```

4. **Access Jupyter Notebook**
   In VSCode, select a new kernel (existing jupyter server) and paste the URL:

📌 Your Jupyter notebooks will now be accessible in VS Code ! You can also create a virtual environment if you do not wish to use a docker image.

5. **Get the animals Dataset**
Go to https://www.kaggle.com/datasets/iamsouravbanerjee/animal-image-dataset-90-different-animals?resource=download and download the dataset. Then put it in the foler animals_dataset/ (you should find the pictures of the animals in animals_dataset/animals/animals/** / *.)
