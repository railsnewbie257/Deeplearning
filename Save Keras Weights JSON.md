https://machinelearningmastery.com/save-load-keras-deep-learning-models/



<pre>
conda install h5py
</pre>

https://keras.io/getting-started/faq/#how-can-i-save-a-keras-model

<b>Save the architecture and weights</b>

<pre>

model.save(<em>filePath</em>)
</pre>

<b>Load architecture and weights, will automatically compile if original save was compiled</b>
<pre>

from keras.model import load_model

model = load_model(<em>filePath</em>)
</pre>
