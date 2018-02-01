# GirlOrBoy
### Intro
Very simple model. I retrained the top layer of the [*Inception v3 model*](https://arxiv.org/pdf/1512.00567.pdf) neural network in order to tell if the person in a given picture was a man or a woman. Tensorflow provides already trained NNs with a retraining python program which allows you to retrain the network to custom classes. The ultimate goal of this project is to integrate this network into a useful program. **FULLY CUSTOM MODEL/TRAINING PROGRAM TO COME**

### Usage
1. Install  [Tensorflow](https://www.tensorflow.org/install/)
2. Place picture you wish to classify in root of repo, or alter path in point 3 (*--image=$HOME/<your photo>*) to desired directory
3. Run following command from tensorflow directory
```
python tensorflow/examples/label_image/label_image.py \
--graph=/tmp/output_graph.pb --labels=/tmp/output_labels.txt \
--input_layer=Mul \
--output_layer=final_result \
--input_mean=128 --input_std=128 \
--image=$HOME/**<your photo>**
```
4. Class probabilities should output to console.

