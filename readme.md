COMP334 Fall 2024 Final Project: Algorithmic Bias in Facial Recognition Software
===
Authors: Rufaida Khan, Julissa Mota, and Gazi Rahman

This repository tests Facenet, a face embedding model, for algorithmic bias based on race and sex. In it, we use `facenet-pytorch`, a wrapper around Facenet, to embed and compare faces from the [Chicago Face Database](https://www.chicagofaces.org). We calculate the distance between each face embedding and every other face embedding; we use the distance between the embeddings to label whether two images pertain to the same person. We store values based on whether two images actually pertain to the same person and what the model predicted.

After having the model perform a pairwise analysis of every possible combination of images, we analyze the results based on race and sex. We test for whether the difference in performance is statistically significant, detailing our thoughts in the formal writeup.

To run the jupyter notebook yourself, please do the following.

1. Ensure that you have Python version 3.3+ downloaded on your machine; we built this project on version 3.12.7. You can check by simply running `python --version`

2. Navigate to the [Chicago Face Database](https://www.chicagofaces.org) and download the dataset. Given the license of the dataset, we are not allowed to distribute the data ourselves but it is very easily accessible; there is an immediate turnaround between submitting the request form and receiving a download link.

3. Move the `CFD Version 3.0/Images/CFD/` folder to the repostory. That is to say, only move folder titled `CFD` contained in the `Images` folder of the download to the repo.

4. Navigate to the project repo in terminal and run `python -m venv venv`.

5. Run `source venv/bin/activate`.

6. Run `pip install -r requirements.txt`.

7. Open the Jupyter Notebook in your manner of choice, select the virtual environment `venv` as the kernel.

8. Modify the `data_path` variable in the notebook according to the location of the dataset on your machine.

9. Run the cells as you wish. We did so using VSCode although this may look different and require some configuring on your end.