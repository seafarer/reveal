<div>
<section>
      <h2>Step 1: Attach Needed Files</h2>
      <script type="text/javascript" src="http://snipt.net/embed/5392cac07bc6cd36b10629561124ca68"></script>  
    </section>

    <section>
      <h2>Step 2: The Modal Markup</h2>
      <pre> /* Attach the Reveal CSS */
        <link rel="stylesheet" href="reveal.css">
        
        /* jQuery needs to be attached */
        <script src="jquery.min.js" type="text/javascript"></script>
        
        /* Then just attach the Reveal plugin */
        <script src="jquery.reveal.js" type="text/javascript"></script>
      </pre>

    </section>

    <section>
      <h2>Step 3: Attaching Your Handler</h2>
      <pre>
        <div id="myModal" class="reveal-modal">
          <h1>Modal Title</h1>
          <p>Any content could go in here.</p>
          <a class="close-reveal-modal">&#215;</a>
        </div>
      </pre>
      <p>By putting the "data-reveal-id" attribute on the anchor, when clicked the plugin matches the value of the "data-reveal-id" attribute (in this case "myModal") with an HTML element with that ID.</p>
      <p class="lead">Basically, put the "data-reveal-id" attribute on an object and make it's value the ID of your modal.</p>
      
      <p>While the "data-reveal-id" is an awesome way to make firing a modal stupid-easy, <strong>in many cases developers will still need to be fired programatically.</strong> That's easy enough too...</p>
    </section>

    <section>
      <h2>Options</h2>
      <p>Every good plugin has options, and this one has just a few, but important ones:</p>
      <pre>
        $('#myModal').reveal({
        animation: 'fadeAndPop',                   //fade, fadeAndPop, none
        animationspeed: 300,                       //how fast animtions are
        closeonbackgroundclick: true,              //if you click background will modal close?
        dismissmodalclass: 'close-reveal-modal'    //the class of a button or element that will close an open modal
     });
      </pre>
      <p><strong>Wondering how to use the options when you're using the "data-reveal-id" implementation</strong>? Basically take the option and add the "data-" before and pass a valid value. Here is it with default values:</p>
      <pre>
        <a href="#" data-reveal-id="myModal" data-animation="fadeAndPop" data-animationspeed="300" data-closeonbackgroundclick="true" data-dismissmodalclass="close-reveal-modal">Click for a modal</a>
      </pre>
    </section>

    <p class="lead">The Reveal plugin is licensed to use and abuse under the MIT license. Ballin!</p>
</div>