<h1 dir="auto"><span>0x00. AirBnB clone - The console</span></h1>
<blockquote>
<h2> Description </h2>
<p dir="auto">This proyect is the implementation of an storeg engine, and how to store all the information about users in a json file, control by a console, as the name mentioned this proyect create a console in interactive and non-interactive mode, and it used to create and implement a lot of command to recreate a storeg engine </p>
</blockquote>
<blockquote>
</ul>
<h2>Serialization-deserialization's flow:</h2>
<p dir="auto">&lt;class 'BaseModel'&gt; -&gt; to_dict() -&gt; &lt;class 'dict'&gt; -&gt; JSON dump -&gt; &lt;class 'str'&gt; -&gt; FILE -&gt; &lt;class 'str'&gt; -&gt; JSON load -&gt; &lt;class 'dict'&gt; -&gt; &lt;class 'BaseModel'&gt;</p>
<p> This is the process of Serialization and deserialization to a json file </p>
<h2> Proyect Overview:</h2>
<img src="https://s3.amazonaws.com/intranet-projects-files/concepts/74/hbnb_step1.png">
