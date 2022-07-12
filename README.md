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
<h3 dir="auto">How to start it:</h3>
<blockquote>
<p dir="auto"><span>AirBnB$ ./console.py</span>&nbsp;"""interactive mode"""</p>
</blockquote>
<p dir="auto">(hbnb) help</p>
<p dir="auto">Documented commands (type help &lt; topic &gt;):</p>
<hr />
<p dir="auto">EOF all create destroy help quit show update</p>
<p dir="auto">(hbnb)</p>
<p dir="auto">(hbnb) quit</p>
<blockquote>
<p dir="auto"><span>AirBnB$ echo "help" | ./console.py</span>&nbsp;"""non-interactive mode""" (hbnb)</p>
</blockquote>
<p dir="auto">Documented commands (type help &lt; topic &gt;):</p>
<blockquote>
<p dir="auto">This is the command's list:</p>
</blockquote>
<ul dir="auto">
<li><span>help</span>&nbsp;- Shows information about the console or its commands - Usage: help or help create</li>
<li><span>EOF</span>&nbsp;- Exits the console</li>
<li><span>quit</span>&nbsp;- Exits the console</li>
<li><span>create</span>&nbsp;- Creates an instance - Usage: create Class</li>
<li><span>show</span>&nbsp;- Prints the string representation of an instance - Usage: show Class id</li>
<li><span>destroy</span>&nbsp;- Deletes an intance - Usage: destroy Class id</li>
<li><span>all</span>&nbsp;- Prints all string representation of all instance - Usage: all or all Class</li>
<li><span>update</span>&nbsp;- Updates an instance - Usage: update Class id attribute value</li>
</ul>
<h3>Examples:</h3>
<p dir="auto"><span>Create:</span></p>
<blockquote>
<p dir="auto">(hbnb) create BaseModel</p>
</blockquote>
<p dir="auto">929fab0f-efb4-4eb7-9cfa-27c57cd167df</p>
<blockquote>
<p dir="auto">(hbnb) create User</p>
</blockquote>
<p dir="auto">5aa4eec2-ce66-4415-ba41-28c3207a68b6</p>
<blockquote>
<p dir="auto">(hbnb) create Place</p>
</blockquote>
<p dir="auto">63514b83-af33-4038-9c66-256fefc35165</p>
<p dir="auto"><span>destroy:</span></p>
<blockquote>
<p dir="auto">(hbnb) create Place</p>
</blockquote>
<p dir="auto">9fd1f506-9cc7-4ba8-9b2f-d6bda9bbcddb</p>
<blockquote>
<p dir="auto">(hbnb) destroy Place 9fd1f506-9cc7-4ba8-9b2f-d6bda9bbcddb</p>
</blockquote>
<blockquote>
<p dir="auto">(hbnb) show Place 9fd1f506-9cc7-4ba8-9b2f-d6bda9bbcddb</p>
</blockquote>
<p dir="auto">** no instance found **</p>
<p dir="auto"><span>all:</span></p>
<blockquote>
<p dir="auto">(hbnb) create BaseModel</p>
</blockquote>
<p dir="auto">bf876ce4-ecc9-4185-8d22-88c23cbe4f28</p>
<blockquote>
<p dir="auto">(hbnb) create BaseModel</p>
</blockquote>
<p dir="auto">61691f4f-f58c-4b58-8618-14472c984061</p>
<blockquote>
<p dir="auto">(hbnb) create User</p>
</blockquote>
<p dir="auto">81fc9995-016a-4f47-85ef-62bb73ce5e1c</p>
<blockquote>
<p dir="auto">(hbnb) all</p>
</blockquote>
<p dir="auto">["[BaseModel] (bf876ce4-ecc9-4185-8d22-88c23cbe4f28) {'id': 'bf876ce4-ecc9-4185-8d22-88c23cbe4f28', 'created_at': datetime.datetime(2022, 7, 6, 15, 49, 15, 483376), 'updated_at': datetime.datetime(2022, 7, 6, 15, 49, 15, 483395)}", "[BaseModel] (61691f4f-f58c-4b58-8618-14472c984061) {'id': '61691f4f-f58c-4b58-8618-14472c984061', 'created_at': datetime.datetime(2022, 7, 6, 15, 49, 31, 624055), 'updated_at': datetime.datetime(2022, 7, 6, 15, 49, 31, 624070)}", "[User] (81fc9995-016a-4f47-85ef-62bb73ce5e1c) {'id': '81fc9995-016a-4f47-85ef-62bb73ce5e1c', 'created_at': datetime.datetime(2022, 7, 6, 15, 49, 36, 876947), 'updated_at': datetime.datetime(2022, 7, 6, 15, 49, 36, 877007)}"]</p>
