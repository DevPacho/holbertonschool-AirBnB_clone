<h1 dir="auto"><span>0x00. AirBnB clone - The console</span></h1>
<h2 dir="auto"><a id="user-content-projects-description" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#projects-description"></a>Project's description:</h2>
<blockquote>
<p dir="auto">This is the first step towards building a full web application: the AirBnB clone. This first step is very important because we will use what we build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration&hellip;</p>
</blockquote>
<blockquote>
<p dir="auto">Steps:</p>
</blockquote>
<ul dir="auto">
<li>Create a parent class (called&nbsp;<span>BaseModel</span>) to take care of the initialization, serialization and deserialization of the future instances.</li>
<li>Create a simple flow of serialization/deserialization: Instance &lt;-&gt; Dictionary &lt;-&gt; JSON string &lt;-&gt; file.</li>
<li>Create all classes used for AirBnB (User, State, City, Place&hellip;) that inherit from BaseModel.</li>
<li>Create the first abstracted storage engine of the project: File storage.</li>
<li>Create all unittests to validate all the classes and storage engine.</li>
<li>Create the command interpreter.</li>
</ul>
<blockquote>
<p dir="auto">Our child classes from BaseModel:</p>
</blockquote>
<ul dir="auto">
<li>User</li>
<li>State</li>
<li>City</li>
<li>Place</li>
<li>Amenity</li>
<li>Review</li>
</ul>
<blockquote>
<p dir="auto">And our class for the engine:</p>
</blockquote>
<ul dir="auto">
<li>FileStorage</li>
</ul>
<h2 dir="auto"><a id="user-content-serialization-deserializations-flow" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#serialization-deserializations-flow"></a>Serialization-deserialization's flow:</h2>
<p dir="auto">&lt;class 'BaseModel'&gt; -&gt; to_dict() -&gt; &lt;class 'dict'&gt; -&gt; JSON dump -&gt; &lt;class 'str'&gt; -&gt; FILE -&gt; &lt;class 'str'&gt; -&gt; JSON load -&gt; &lt;class 'dict'&gt; -&gt; &lt;class 'BaseModel'&gt;</p>
<blockquote>
<p dir="auto">For this first step, we have to write in a file all our objects/instances created/updated in our command interpreter and restore them when we start it. We can&rsquo;t store and restore a Python instance of a class as &ldquo;Bytes&rdquo;, the only way is to convert it to a serializable data structure as the one above.</p>
</blockquote>
<h2 dir="auto"><a id="user-content-command-interpreter" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#command-interpreter"></a>Command Interpreter:</h2>
<blockquote>
<p dir="auto">The console allow us to create the data model, manage objects and store and persist objects to a file (JSON file). Some examples:</p>
</blockquote>
<ul dir="auto">
<li>Create a new object (ex: a new User or a new Place).</li>
<li>Retrieve an object from a file, a database etc&hellip;</li>
<li>Do operations on objects (count, compute stats, etc&hellip;).</li>
<li>Update attributes of an object.</li>
<li>Destroy an object.</li>
</ul>
<blockquote>
<p dir="auto">The first piece is to manipulate the storage system. This storage engine will give us an abstraction between &ldquo;Our objects&rdquo; and &ldquo;How they are stored and persisted&rdquo;. This means: from our console code (the command interpreter itself) and from the front-end and RestAPI we will build later, we won&rsquo;t have to pay attention (take care) of how our objects are stored. This abstraction will also allow us to change the type of storage easily without updating all of our codebase.</p>
</blockquote>
<blockquote>
<p dir="auto">The console will be a tool to validate this storage engine.</p>
</blockquote>
<h2 dir="auto"><a id="user-content-first-approach-to-the-project" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#first-approach-to-the-project"></a>First approach to the project:</h2>
<p><a href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/AirBnBv1.png?raw=true" rel="noopener noreferrer" target="_blank"><img src="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/raw/master/AirBnBv1.png?raw=true" alt="Stage1-AirBnB_clone_project" /></a></p>
<h3 dir="auto"><a id="user-content-how-to-start-it" class="anchor" href="https://github.com/jhojanperlaza/holbertonschool-AirBnB_clone/blob/master/README.md#how-to-start-it"></a>How to start it:</h3>
<blockquote>
<p dir="auto"><span>AirBnB$ ./console.py</span>&nbsp;"""interactive mode"""</p>
</blockquote>
<p dir="auto">(hbnb) help</p>
<p dir="auto">Documented commands (type help &lt; topic &gt;):</p>
