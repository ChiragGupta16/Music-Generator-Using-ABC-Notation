# Music Generation Using RNN
<h2> Generated Music</h2>
<p>
  Stream the music on vimeo for free. <br>
  Link -> https://vimeo.com/948299931
</p>

<h2> Overview</h2>
<p>
  Tired of getting the same code everywhere ? <br>
  Here is something different from the ones using midi files :) <br>
  This code generates music using ABC Notation. They are also known as Sheet Notation. Its the same thing a 
pianist sees while playing piano. The model is based on RNN to predict the the next note. <br>
  It is made using tensorflow and keras.
</p>
<h2>Data Source and Libraries</h2>
<p>
  I have used the ABC Notation files from Nottingham Music Database(https://abc.sourceforge.net/NMD/) <br>
  It contains over 1000 Folk Tunes stored in a special ABC format. Do check it out!<br>
  You can use any tune for training<br><br>
  For converting the abc format text to music we will use <b>music21</b> library. You can get the documentation here(https://web.mit.edu/music21/doc/) <br>
  We will also use <b>abcjs</b> to download midi files generated from ABC Notation. You will find the link of the website inside the file.
  <b>ChatGPT</b> will also be used to check uniform line breaks in generated notation to save time.
</p>
<h2>General Idea</h2>
<p>
  We will download the data set from the <b>Nottingham Music Database</b>. <br>
  During preprocessing, we will remove unnecessary lines and notation. We will then play the music using <b>music21</b> library. <br>
  We will then convert each token in the data set to a unique number. Then these numbers will be fed into the model based on RNN. <br>
  After the traing is completed we will join the generated text with the original text and convet it back to ABC Notation.
  It is then checked for missing puncuations using ChatGPT to save manual labour.<br>
  The updated notation is then played on a website based on <b>abcjs</b> and we will download it from the website.
</p> 
<h4>Note :</h4><p>Increase the epoch while training for better result.</p>
<h4>Happy Coding !!</h4>
