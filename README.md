# fcc-timestamp-microservice
FreeCodeCamp APIs and Microservices Projects - Timestamp Microservice
<header>
        <h1>API Project: Timestamp Microservice</h1>
      </header>
      <section>
        <h3>User Stories (WIP):</h3>
        <ol>
          <li>
            <p>The API endpoint is <code>GET [project_url]/api/timestamp/:date_string?</code></p>
          </li>
          <li>
            <p>A date string is valid if can be successfully parsed by <code>new Date(date_string)</code>.
            Note that the unix timestamp needs to be an integer (not a string) specifying milliseconds.
            In our test we will use date strings compliant with ISO-8601 (e.g. "2016-11-20") because this will ensure an UTC timestamp.</p>
          </li>
          <li>
            <p>If the date string is empty it should be equivalent to trigger <code>new Date()</code>, i.e. the service uses the current timestamp.</p>
          </li>
          <li>
            <p>If the date string is valid the api returns a JSON having the structure
            <code>{"unix": &lt;date.getTime()&gt;, "utc" : &lt;date.toUTCString()&gt; }</code>
            e.g. <code>{"unix": 1479663089000 ,"utc": "Sun, 20 Nov 2016 17:31:29 GMT"}</code></p>
          </li>
          <li>
            <p>If the date string is invalid the api returns a JSON having the structure
            <code>{"error" : "Invalid Date" }</code>.</p>
          </li>
        </ol>
      </section>
      <section>
        <h3>Example Usage:</h3>
        <ul>
          <li><p><a href="/api/timestamp/2015-05-30">[project_url]/api/timestamp/2015-05-30</a></p></li>
          <li><p><a href="/api/timestamp/1432944066985">[project_url]/api/timestamp/1432944066985</a></p></li>
        </ul>
      </section>
      <section>
        <h3>Example Output:</h3>
        <ul>
          <li><p><code>{"unix":1432944000000,"utc":"Sat, 30 May 2015 00:00:00 GMT"}</code></p></li>
          <li><p><code>{"unix":1432944066985,"utc":"Sat, 30 May 2015 00:01:06 GMT"}</code></p></li>
        </ul>
      </section>
      <footer>
        <p>By <a href="https://www.freecodecamp.org/" target="__blank">freeCodeCamp</a></p>
        <p>
          <span>Check live on <a href="https://i-anshuman-fcc-timestamp-microservice.glitch.me" target="__blank">Glitch</a></span>
          <span>Check source on <a href="https://github.com/i-anshuman/fcc-timestamp-microservice" target="__blank">Github</a></span>
        </p>
      </footer>
