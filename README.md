<h1 dir="auto"><span>0x00. AirBnB clone - The console</span></h1>
<blockquote>
<h2> Description </h2>
<p dir="auto">This proyect is the implementation of an storeg engine, and how to store all the information about users in a json file, control by a console, as the name mentioned this proyect create a console in interactive and non-interactive mode, and it used to create and implement a lot of command to recreate a storeg engine </p>
</blockquote>
<blockquote>
</ul>
<h2 dir="auto"><a id="user-content-serialization-deserializations-flow" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#serialization-deserializations-flow"></a>Serialization-deserialization's flow:</h2>
<p dir="auto">&lt;class 'BaseModel'&gt; -&gt; to_dict() -&gt; &lt;class 'dict'&gt; -&gt; JSON dump -&gt; &lt;class 'str'&gt; -&gt; FILE -&gt; &lt;class 'str'&gt; -&gt; JSON load -&gt; &lt;class 'dict'&gt; -&gt; &lt;class 'BaseModel'&gt;</p>
<blockquote>
<p dir="auto"> This is the process of Serialization and deserialization to a json file </p>
</blockquote>
<p dir="auto">The console will be a tool to validate this storage engine.</p>
</blockquote>
<h2 Proyect Overview:</h2>
<p><a href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/AirBnBv1.png?raw=true" rel="noopener noreferrer" target="_blank"><img src="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/raw/master/AirBnBv1.png?raw=true" alt="Stage1-AirBnB_clone_project" /></a></p>
<h3 dir="auto"><a id="user-content-how-to-start-it" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#how-to-start-it"></a>How to start it:</h3>
<blockquote>
<p dir="auto"><span>AirBnB$ ./console.py</span>&nbsp;"""interactive mode"""</p>
</blockquote>
<p dir="auto">(hbnb) help</p>
<p dir="auto">Documented commands (type help &lt; topic &gt;):</p>
