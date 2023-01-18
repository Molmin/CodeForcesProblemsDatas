## Description

<div><p>You are given a <a href="https://assets.codeforces.com/rounds/1357/training_data3.json">training dataset</a>, in which each entry is a features vector (an array of 2 real numbers) and a label 0 or 1 indicating the class to which this vector belongs.</p><p>Your goal is to use this dataset to train a quantum classification model that will accurately classify a validation dataset - a different dataset generated using the same data distribution as the training one. The error rate of classifying the validation dataset using your model (the percentage of incorrectly classified samples) should be less than 5%.</p><ul> <li> The quantum classification library that will use your model to classify the data is documented <a href="https://docs.microsoft.com/quantum/libraries/machine-learning/">here</a>. </li><li> <a href="https://github.com/microsoft/MLADS2020-QuantumClassification">This tutorial</a> has an end-to-end example of training a model using this library as a Python notebook. </li><li> The <a href="https://codeforces.com/blog/entry/78832">warmup round editorial</a> discusses solving easier problems features in the warmup round. </li><li> <span class="tex-font-style-bf">You can find the exact implementation of the testing harness for the D problems of this round, including the preprocessing methods, <a href="https://github.com/tcNickolas/MiscQSharp/tree/master/CodingContest2020-QML">here</a>.</span> </li><li> You can find examples of training a model and using it for classification <a href="https://github.com/microsoft/Quantum/tree/master/samples/machine-learning/">here</a>. </li></ul></div><div class="input-specification"><p>Your code will not be given any inputs. Instead, you should use the <a href="https://assets.codeforces.com/rounds/1357/training_data3.json">provided dataset file</a> to train your model.</p><p>The training dataset is represented as a JSON file and consists of two arrays, "Features" and "Labels". Each array has exactly 400 elements. Each element of the "Features" array is an array with 2 elements, each of them a floating-point number. Each element of the "Labels" array is the label of the class to which the corresponding element of the "Features" array belongs, 0 or 1.</p></div><div class="output-specification"><p>Your code should return the description of the model you'd like to use in the following format:</p><ul> <li> The model is described using a tuple <span class="tex-font-style-tt">((Int, Double[]), ControlledRotation[], (Double[], Double))</span>. </li><li> The first element of the tuple describes the classical preprocessing you perform on the data before encoding it into the quantum classifier. </li><li> The second element of the tuple describes circuit geometry of the model as an array of controlled rotation gates. </li><li> The third element of the tuple describes numeric parameters of the model and is a tuple of an array of rotation angles used by the gates and the bias used to decide the class of the model. </li></ul><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {<br>    open Microsoft.Quantum.MachineLearning;<br><br>    operation Solve () : ((Int, Double[]), ControlledRotation[], (Double[], Double)) {<br>        // your code here<br>    }<br>}</pre><p><span class="tex-font-style-bf">Classical preprocessing</span></p><p>This step allows you to add new features to the data before encoding it in the quantum state and feeding it into the classifier circuit. To do this, you need to pick one of the available preprocessing methods and return a tuple of its index and its parameters. The parameters of all methods are <span class="tex-font-style-tt">Double[]</span>.</p><ul> <li> <span class="tex-font-style-bf">Method 1: padding.</span> The resulting data is a concatenation of the parameters and the features. </li><li> <span class="tex-font-style-bf">Method 2: tensor product.</span> The resulting data is an array of pairwise products of the elements of the parameters and the features. </li><li> <span class="tex-font-style-bf">Method 3: fanout.</span> The resulting data is a tensor product of the parameters, the features and the features (so that you have access to all pairwise products of features). </li><li> <span class="tex-font-style-bf">Method 4: split fanout.</span> The resulting data is tensor product of (concatenation of the left halves of parameters and features) and (concatenation of the right halves). </li><li> <span class="tex-font-style-bf">Default method: no preprocessing.</span> The features remain unchanged, the parameters are ignored. This method is used when any index other than 1-4 is returned. </li></ul><p>After the preprocessing step the resulting data is encoded in the quantum state using amplitudes encoding: element $j$ of the data is encoded in the amplitude of basis state $|j\rangle$. If the length of the data array is not a power of 2, it is right-padded with $0$s to the nearest power of two; the number of qubits used for encoding is the exponent of that power.</p></div>

## Input

<p>Your code will not be given any inputs. Instead, you should use the <a href="https://assets.codeforces.com/rounds/1357/training_data3.json">provided dataset file</a> to train your model.</p><p>The training dataset is represented as a JSON file and consists of two arrays, "Features" and "Labels". Each array has exactly 400 elements. Each element of the "Features" array is an array with 2 elements, each of them a floating-point number. Each element of the "Labels" array is the label of the class to which the corresponding element of the "Features" array belongs, 0 or 1.</p>

## Output

<p>Your code should return the description of the model you'd like to use in the following format:</p><ul> <li> The model is described using a tuple <span class="tex-font-style-tt">((Int, Double[]), ControlledRotation[], (Double[], Double))</span>. </li><li> The first element of the tuple describes the classical preprocessing you perform on the data before encoding it into the quantum classifier. </li><li> The second element of the tuple describes circuit geometry of the model as an array of controlled rotation gates. </li><li> The third element of the tuple describes numeric parameters of the model and is a tuple of an array of rotation angles used by the gates and the bias used to decide the class of the model. </li></ul><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {<br>    open Microsoft.Quantum.MachineLearning;<br><br>    operation Solve () : ((Int, Double[]), ControlledRotation[], (Double[], Double)) {<br>        // your code here<br>    }<br>}</pre><p><span class="tex-font-style-bf">Classical preprocessing</span></p><p>This step allows you to add new features to the data before encoding it in the quantum state and feeding it into the classifier circuit. To do this, you need to pick one of the available preprocessing methods and return a tuple of its index and its parameters. The parameters of all methods are <span class="tex-font-style-tt">Double[]</span>.</p><ul> <li> <span class="tex-font-style-bf">Method 1: padding.</span> The resulting data is a concatenation of the parameters and the features. </li><li> <span class="tex-font-style-bf">Method 2: tensor product.</span> The resulting data is an array of pairwise products of the elements of the parameters and the features. </li><li> <span class="tex-font-style-bf">Method 3: fanout.</span> The resulting data is a tensor product of the parameters, the features and the features (so that you have access to all pairwise products of features). </li><li> <span class="tex-font-style-bf">Method 4: split fanout.</span> The resulting data is tensor product of (concatenation of the left halves of parameters and features) and (concatenation of the right halves). </li><li> <span class="tex-font-style-bf">Default method: no preprocessing.</span> The features remain unchanged, the parameters are ignored. This method is used when any index other than 1-4 is returned. </li></ul><p>After the preprocessing step the resulting data is encoded in the quantum state using amplitudes encoding: element $j$ of the data is encoded in the amplitude of basis state $|j\rangle$. If the length of the data array is not a power of 2, it is right-padded with $0$s to the nearest power of two; the number of qubits used for encoding is the exponent of that power.</p>

## Note

<p>Note that majority of the data analysis is going to happen "offline" before you submit the solution. The solution has to contain only the description of the trained model, not the training code itself - if you attempt to train the model "online" in your submitted code during the evaluation process, it will very likely time out.</p><p>Training your model offline is likely to involve:</p><ul> <li> Defining the circuit structure that your model will use. </li><li> Generating several parameter seed vectors - the values from which training the model will start. </li><li> Selecting appropriate hyperparameters of the training process (learning rate, batch size, tolerance, maximal number of iterations etc.) </li><li> Training a number of classification models (one per each seed vector and hyperparameter combination) </li><li> Selecting the best trained model and submitting it. </li></ul>