<h1>K-Means Clustering with TensorFlow</h1>

<p>This repository demonstrates the implementation of K-Means clustering using TensorFlow for optimization, with random initialization of centroids and Adam optimizer.</p>

<h2>Features</h2>
<ul>
  <li>Generate 1500 samples with 2 features and 3 clusters using <code>make_blobs</code></li>
  <li>Use TensorFlow's <code>GradientTape</code> and <code>Adam optimizer</code> to optimize centroids</li>
  <li>Dynamic cluster assignment and loss calculation based on Euclidean distance</li>
  <li>Visualization using <code>matplotlib</code> with adjustable color maps and centroid markers</li>
</ul>

<h2>Steps</h2>
<ol>
  <li>Initialize centroids randomly.</li>
  <li>For each epoch:
    <ul>
      <li>Assign clusters based on minimum distance.</li>
      <li>Calculate the loss (sum of squared distances to centroids).</li>
      <li>Apply gradients to optimize centroids.</li>
    </ul>
  </li>
  <li>Plot the data points and centroids with customizable appearance (color map and marker size).</li>
</ol>

<h2>Loss Function</h2>
<p>The loss function used is the sum of squared distances between data points and their corresponding centroids:</p>
<p><code>loss = Σ (x<sub>i</sub> - c<sub>k<sub>i</sub></sub>)<sup>2</sup></code></p>

<h2>Plotting</h2>
<p>The scatter plot displays the data points colored based on their assigned cluster, with centroids marked as black 'X'. The color map is customizable to make the centroids stand out more clearly.</p>

<h2>Customization</h2>
<ul>
  <li>Adjust the learning rate with the <code>learning_rate</code> parameter.</li>
  <li>Change the number of epochs to control training duration.</li>
  <li>Modify the size and style of the centroid markers using the <code>marker</code> and <code>linewidths</code> parameters in <code>matplotlib</code>.</li>
</ul>

<h2>Dependencies</h2>
<ul>
  <li><code>tensorflow</code></li>
  <li><code>matplotlib</code></li>
  <li><code>numpy</code></li>
  <li><code>scikit-learn</code></li>
</ul>
