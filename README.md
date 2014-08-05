# TickerMePink

A lightweight (<4k), customizable news ticker plugin for jQuery. It uses hard-coded SVG control buttons so no extra images are needed. All you need is the plugin.

## Version

1.0

## Usage

### i. Include jQuery and the plugin:

```
<script type="text/javascript" src="assets/js/jquery-1.11.1.min.js"></script>
<script type="text/javascript" src="assets/js/tickerme.min.js"></script>
```

### ii. Add your news stories in a list:

You can give the wrapper any `id` - in this case we're using `ticker`.

```
<ul id="ticker">
	<li>This is the first news story.</li>
	<li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente, molestiae.</li>
	<li>Another news story.</li>
	<li>The final news story, with some more test text.</li>
</ul>
```

### iii. Call the plugin with your wrapper id:

```
$(function(){
	$('#ticker').tickerme();
});
```

### iv: Optional - edit the TickerMePink's style:

You can edit the way TickerMePink wraps the ticker: either create a definition in your CSS file for `#ticker_container`, or edit the one provided in the example `styles.css`:

```
#ticker_container {
	padding:10px;
	border:1px solid #676767;
	-webkit-border-radius: 7px;
	-moz-border-radius: 7px;
	border-radius: 7px;
	overflow: auto;
}
```

## Options

### fade_speed

The speed each story will fade in and out (milliseconds).
Default: `500`

### duration

The length of time a story is on the screen (milliseconds).
Default: `3000`

### auto_stop

If `true`, the ticker will automatically stop when the previous or next button is clicked.
Default: `true`

### control_colour

The colour of the play, pause, previous and next controls.
Default: `#333333`

### control_rollover 

The colour of the control buttons on rollover.
Default: `#666666`

## Example:

```
$(function(){
	$('#news_stories').tickerme({
		fade_speed: 900,
		auto_stop: false,
		control_rollover: '#FF0000'
	});
});
```

 
