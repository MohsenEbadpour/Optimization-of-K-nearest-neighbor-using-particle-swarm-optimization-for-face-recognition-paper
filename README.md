# Optimization of K-Nearest Neighbor for Face Recognition using Particle Swarm Optimization

This project is an implementation of the paper "Optimization of K-nearest neighbor using particle swarm optimization for face recognition" in Python, with a focus on using Principal Component Analysis (PCA) instead of Local Binary Patterns (LBP). The ORL face database was used.

The paper proposes an optimization method for the k-nearest neighbor (k-NN) algorithm using particle swarm optimization (PSO) to select the optimal number of neighbor for classification and selecting features. The authors compare the results of PSO with those of other optimization algorithms, including ant colony optimization (ACO) and genetic algorithm (GA), and show that PSO performs better in term of accuracy.

In this project, PCA is used for feature extraction instead of LBP, and a custom PCA algorithm is implemented that selects only a subset of the eigenvectors based on a PSO optimization process. The accuracy of the k-NN algorithm is then maximized using PSO to select the best subset of eigenvectors.

The project is organized into separate Jupyter notebooks for each stage of the process, including data preprocessing, PCA, k-NN, ACO, GA, and PSO. The code can be easily run on the ORL database or adapted for other face recognition tasks.

## Results

Our experiments show that using custom PCA with PSO to select the best subset of eigenvectors for K-NN significantly (not only top eigenvectors) improves the accuracy of face recognition on the ORL dataset. We achieved an accuracy of 97.1% on the testing set, which is higher than the accuracy achieved using other mentioned algorithms.

## Usage
To use this code, you will need to install Python 3 and the following libraries:

- numpy
- pandas
- matplotlib
- seaborn
- glob
- cv2
- skimage
- sklearn
- sklearn_genetic
- pyswarms


Once you have installed the required libraries, you can run the Jupyter notebooks in order to preprocess the data, perform custom PCA, and run K-NN with custom PCA.

## Credits

This code is inspired by the paper "Optimization of K-Nearest Neighbor using Particle Swarm Optimization for Face Recognition" by XYZ et al.

## License

This project is licensed under the GPL-3.0 License.

## Information

This Project is related to a *Statistical Pattern Recognition* course taught by Professor Mohammad Rahmati (<rahmati@aut.ac.ir>) in the Computer Engineering department at Amirkabir University of Technology (AUT) in Tehran, Iran. The course was offered in the Fall of 2021. The project was my final project in mentioned course.

## Feedback

If you have any feedback or suggestions for improving this code, please feel free to open an issue in the repository as well as send an email to Mohsen Ebadpour (<m.ebadpour@aut.ac.ir> , <mohsenebadpour@outlook.com>).

