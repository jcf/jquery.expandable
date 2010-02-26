# jquery.expandable

Created by James Conroy-Finn.

This plugin is ultimately simple, it takes no arguments and assumes you simply want to have a "view port" hide the contents of a big child until a user clicks on the "view port".

## Usage

Wrap your large, element in a DIV...

    <div class="view_port">
      <div>
        <h1>Some content</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur magna aliqua. Ut enim ad minim 
          veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea 
          commodo consequat. Duis aute irure dolor in reprehenderit in voluptate 
          velit esse cillum dolore eu fugiat nulla pariatur.  Excepteur sint 
          occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
          mollit anim id est mega peng
        </p>
      </div>
    </div>

Define the height for your view port in your CSS and add some optional styles to use when your "view port" is expanded...

    .view_port { height: 18px; background-color: #eee; }
    .view_port.expanded { background-color: #fff };

Or in your SASS if you're anything like me!

    .view_port
      height: 18px
      background-color: #eee

      &.expanded
        background-color: #fff

Then in your JS somewhere call expandable on a jQuery selection...

    $('.view_port').expandable();

