# Awkward Showcase - A jQuery Plugin

Awkward Showcase is a plugin for the JavaScript Framework [jQuery](http://jquery.com). We call it a Content Slider. But it can do more then just slide the content. For example you can add tooltips, enable thumbnails, activate dynamic height and lots more.

Since version 1.0 it's integrated with our Viewline Plugin enabling new innovative ways for displaying content on your website.

## Some Nice Features
**Compatibility**
Compatible with all the Major Browsers (Win & Mac).

**Captions**
Advanced positioning with different animations.

**Tooltips**
Position tooltips based on x- and y-coordinates.

**Thumbnails**
Enable thumbnails, both horizontal and vertical.

**100% CSS**
The look of Awkward Showcase is 100% customizable via CSS.

**View Modes**
Different View Modes (now integrated with Viewline).

**Dynamic Height**
Enabling the showcase to change height based on content.

**Easy Implementations**
The showcase i easy to implement and very easy to customize in CSS.

**Lots more**
A slide can contain any type of HTML element. It's an infinity slide. Etc.

## Implementation Example

    <!DOCTYPE html>
    <html>
    <head>
    <title>Awkward Showcase - Demo #1</title>
    <link rel="stylesheet" href="css/style.aw-showcase.css" />
    <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.5.2/jquery.min.js"></script>
    <script type="text/javascript" src="jquery.aw-showcase.min.js"></script>
    <script type="text/javascript">
    $(document).ready(function()
    {
        $("#showcase").awShowcase(
        {
            content_width:  700,
            content_height: 470
        });
    });
    </script>
    </head>
    <body>
 
    <div id="showcase" class="showcase">
        <!-- Each child div in #showcase represents a slide -->
        <div class="showcase-slide">
            <!-- Put the slide content in a div with the class .showcase-content -->
            <div class="showcase-content">
                <!-- If the slide contains multiple elements you should wrap them in a div with the class
                .showcase-content-wrapper. We usually wrap even if there is only one element,
                because it looks better. -->
                <div class="showcase-content-wrapper">
                    <img src="images/01.jpg" alt="01" />
                </div>
            </div>
            <!-- Put the caption content in a div with the class .showcase-caption -->
            <div class="showcase-caption">
                The Caption
            </div>
            <!-- Put the tooltips in a div with the class .showcase-tooltips. -->
            <div class="showcase-tooltips">
                <!-- Each anchor in .showcase-tooltips represents a tooltip.
                The coords attribute represents the position of the tooltip. -->
                <a href="http://www.awkward.se" coords="634,130">
                    <!-- The content of the anchor-tag is displayed in the tooltip. -->
                    This is a tooltip that displays the anchor html in a nice way.
                </a>
                <a href="http://www.awkward.se" coords="356, 172">
                    <!-- You can add multiple elements to the anchor-tag which are display in the tooltip. -->
                    <img src="images/glasses.png" />
                    <span style="display: block; font-weight: bold; padding: 3px 0 3px 0; text-align: center;">
                        White Glasses: 500$
                    </span>
                </a>
            </div>
        </div>
        <div class="showcase-slide">
            <div class="showcase-content">
                <div class="showcase-content-wrapper">
                    Content...
                </div>
            </div>
        </div>
    </div>
 
    </body>
    </html>


## Configuration Options

<table id="options" cellpadding="0" cellspacing="0">
	<col />
	<col />
	<col width="120" />
	<tr>
		<th>Property</th>
		<th>Default</th>
		<th>Options</th>
	</tr>
	<tr>
		<td>content_width</td>
		<td>700</td>
		<td> </td>
	</tr>
	<tr>
		<td>content_height</td>
		<td>400</td>
		<td> </td>
	</tr>
	<tr>
		<td>fit_to_parent</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>auto</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>interval</td>
		<td>3000</td>
		<td> </td>
	</tr>
	<tr>
		<td>continuous</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>loading</td>
		<td>true</td>
		<td> </td>
	</tr>
	<tr>
		<td>tooltip_width</td>
		<td>200</td>
		<td> </td>
	</tr>
	<tr>
		<td>tooltip_icon_width</td>
		<td>32</td>
		<td> </td>
	</tr>
	<tr>
		<td>tooltip_icon_height</td>
		<td>32</td>
		<td> </td>
	</tr>
	<tr>
		<td>tooltip_offsetx</td>
		<td>18</td>
		<td> </td>
	</tr>
	<tr>
		<td>tooltip_offsety</td>
		<td>0</td>
		<td> </td>
	</tr>
	<tr>
		<td>arrows</td>
		<td>true</td>
		<td> </td>
	</tr>
	<tr>
		<td>buttons</td>
		<td>true</td>
		<td> </td>
	</tr>
	<tr>
		<td>btn_numbers</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>keybord_keys</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>mousetrace</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>pauseonover</td>
		<td>true</td>
		<td> </td>
	</tr>
	<tr>
		<td>stoponclick</td>
		<td>true</td>
		<td> </td>
	</tr>
	<tr>
		<td>transition:</td>
		<td>vslide</td>
		<td>'vslide', 'hslide' or 'fade'</td>
	</tr>
	<tr>
		<td>transition_delay:</td>
		<td>300</td>
		<td> </td>
	</tr>
	<tr>
		<td>transition_speed:</td>
		<td>500</td>
		<td> </td>
	</tr>
	<tr>
		<td>show_caption:</td>
		<td>onload</td>
		<td>'onload', 'onhover' or 'show'</td>
	</tr>
	<tr>
		<td>thumbnails:</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>thumbnails_position:</td>
		<td>outside-last</td>
		<td>'outside-last', 'outside-first', 'inside-last' or 'inside-first'</td>
	</tr>
	<tr>
		<td>thumbnails_direction:</td>
		<td>vertical</td>
		<td>'vertical' or 'horizontal'</td>
	</tr>
	<tr>
		<td>thumbnails_slidex:</td>
		<td>0</td>
		<td>0 = auto / 1 = slide one thumbnail / 2 = slide two thumbnails / etc.</td>
	</tr>
	<tr>
		<td>dynamic_height:</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>speed_change:</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>viewline:</td>
		<td>false</td>
		<td> </td>
	</tr>
	<tr>
		<td>custom_function</td>
		<td>null</td>
		<td> </td>
	</tr>
	<tr>
		<td>custom_transition</td>
		<td>null</td>
		<td> </td>
	</tr>
</table>

