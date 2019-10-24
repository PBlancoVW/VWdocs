# Configuration

## Themes

#### Click to change between dark and light mode

<div class="change-theme-button">
  <input type="image" src="_media/contrast-circle.png" style="height:20px;width:20px"/>
</div>

#### Click to preview other themes

<div class="preview-theme-links">
  <a data-theme="vue">vue.css</a><br/>
  <a data-theme="buble">buble.css</a><br/>
  <a data-theme="dark">dark.css</a><br/>
  <a data-theme="pure">pure.css</a><br/>
</div>

<style>
  .preview-theme-links a:hover {
    cursor: pointer;
    text-decoration: underline;
  }
</style>

<script>
  var changeThemeButton = Docsify.dom.find('.change-theme-button');
  var previewThemeLinks = Docsify.dom.find('.preview-theme-links');
  var themes = Docsify.dom.findAll('[rel="stylesheet"]');

  changeThemeButton.onclick = function (e) {
	var darkDisabled = 0;

	themes.forEach(function (theme) {
		if(theme.title == "dark" && theme.disabled)
			darkDisabled = 1;
	});

	themes.forEach(function (theme) {
		if(darkDisabled == 1) {
			theme.disabled = theme.title !== "dark";
		} else {
			theme.disabled = theme.title !== "vue";
		}
	});
  };

  previewThemeLinks.onclick = function (e) {
    var title = e.target.getAttribute('data-theme')

    themes.forEach(function (theme) {
      theme.disabled = theme.title !== title
    });
  };
</script>

