<h1>XSS example</h1>

<p> Script tags are one of the main vulnerabilities that appear on websites. </p>

<p> One example of cross-site scripting (XSS) can appear when there is weak JavaScript written in "element.innerHMTL". 
    A malicious user can take advantage of this script and input anything inside it. For example they can use put a script such as: </p>
    
<p> 
  <script> 
    const firstName = "<img src='x' alt="maliciousImage" onerror='alert(1)'>";
      </p>
 <p>
    el.innerHTML = firstName; // displays an alert message
  </script>
    </p>
