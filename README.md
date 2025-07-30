Links are the backbone of the web—they allow users to navigate between pages, websites, or different sections of the same page

# 1. Creating a Basic Link

       <a href="https://example.com">Visit Example</a>
       
> Key Attribute: href

Attribute    	Description
> href	       Destination URL for the link

> target       Where to open the link (_blank)

> title        Tooltip shown on hover

 Output: Clicking opens the provided URL.

 # 2. Absolute vs Relative URLs
 
>  Absolute Link
Links to a full external address, starting with http://, https://, or another protocol:

          <a href="https://google.com">Google</a>
          
> Used for linking to external websites

> Always includes protocol and domain

# Relative Link

Links to another file within your own project:

      <a href="about.html">About Us</a>
      <a href="/contact">Contact</a>
      <a href="../home.html">Back to Home</a>
      
Type	         Meaning
> about.html	  Same folder

> ../page	      Go one folder up

> /page       	Root-relative path (from domain root)

 Ideal for internal navigation in your project.

#  3. Default Link Styling

Browsers apply these by default:

> a: blue + underlined

> a:visited: purple

> a:hover: changes color on hover

> a:active: while being clicked

You can override this with CSS.

# 4. Styling Link States

        a {
        text-decoration: none;
        color: #1e90ff;
        font-weight: 500;
      }

        a:hover {
             color: #0056b3;
             text-decoration: underline;
       }

       a:visited {
            color: #6a5acd;
       }

       a:focus {
           outline: 2px dashed #ff9800;
           outline-offset: 4px;
       }

      a:active {
          color: red;
      }
    
 These pseudo-classes allow rich interaction and feedback.

 # Link States Order
 
Always follow the LoVe HAte order:

> :link

> :visited

> :hover

> :active

 Putting them out of order can cause unexpected behavior in styles.

 # 5. Open Links in New Tab
 
            <a href="https://github.com" target="_blank" rel="noopener noreferrer">GitHub</a>
            
Attribute                  	           Use
> target="_blank"      	            Opens link in new tab

> rel="noopener noreferrer"	        Prevents security risks (recommended)

#  Example: Stylish Navigation Menu

           <nav>
              <a href="/">Home</a>
              <a href="/services">Services</a>
              <a href="/contact">Contact</a>
          </nav>
          
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #222;
            padding: 8px 12px;
            border-radius: 5px;
            transition: 0.3s;
        }

        nav a:hover {
              background-color: #f0f0f0;
         }

          nav a:focus {
               outline: 2px solid #1e90ff;
           }
           
 Smooth, accessible, and user-friendly!

 # 6. Accessibility & Usability Tips
 
> Use descriptive link text: Avoid “Click here”

    “Download Resume”  “Click this”
    
> Add title for extra info:

     <a href="/privacy" title="Read our privacy policy">Privacy Policy</a>
     
> Use :focus styles for keyboard navigation

> Avoid nesting block-level tags like <div> inside <a> (use <button> when needed)

# ture	                  Description
> a href="..."              Creates a hyperlink

> Absolute vs Relative	   External vs internal path navigation

> target="_blank"	         Opens link in new tab

> Pseudo-classes	         Style interactive states: hover, visited, etc.

> rel="noopener"         	 Improves security for external tabs




 






