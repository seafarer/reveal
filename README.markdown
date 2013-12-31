<div>
<section>

## Step 1: Attach Needed Files

  <pre>
    /* Attach the Reveal CSS */
    <link rel="stylesheet" href="reveal.css">

    /* jQuery needs to be attached */
    <script src="jquery.min.js" type="text/javascript"></script>

    /* Then just attach the Reveal plugin */
    <script src="jquery.reveal.js" type="text/javascript"></script>
  </pre>
</section>

<section>

## Step 2: The Modal Markup

  <pre> /* Attach the Reveal CSS */
    <div id="myModal" class="reveal-modal">

# Modal Title

Any content could go in here.

     <a class="close-reveal-modal">&#215;</a>
    </div>
  </pre>

</section>

<section>

## Step 3: Attaching Your Handler

  <pre>
    [Click Me For A Modal](#)
  </pre>

By putting the "data-reveal-id" attribute on the anchor, when clicked the plugin matches the value of the "data-reveal-id" attribute (in this case "myModal") with an HTML element with that ID.

Basically, put the "data-reveal-id" attribute on an object and make it's value the ID of your modal.

While the "data-reveal-id" is an awesome way to make firing a modal stupid-easy, **in many cases developers will still need to be fired programatically.** That's easy enough too...

</section>

<section>

## Options

Every good plugin has options, and this one has just a few, but important ones:

  <pre>
    $('#myModal').reveal({
    animation: 'fadeAndPop',                   //fade, fadeAndPop, none
    animationspeed: 300,                       //how fast animtions are
    closeonbackgroundclick: true,              //if you click background will modal close?
    dismissmodalclass: 'close-reveal-modal'    //the class of a button or element that will close an open modal
 });
  </pre>

**Wondering how to use the options when you're using the "data-reveal-id" implementation**? Basically take the option and add the "data-" before and pass a valid value. Here is it with default values:

  <pre>
    [Click for a modal](#)
  </pre>
</section>

The Reveal plugin is licensed to use and abuse under the MIT license. Ballin!

</div>