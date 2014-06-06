Gnome-Shell-Panel-World-Clock
=============================
<i>
Unofficial fork of https://extensions.gnome.org/extension/697/panel-world-clock/ -- Disclaimer: I am NOT the author, but I could not find anywhere the author has this hosted, and I wanted to make a change. Master will represent the version released on extensions.gnome.org. I will keep my changes in branches.
</i>

fixed for gnome-shell 3.10

### todo
  * I had to disable the destruction of the buttons due to the following error:
 
  ``Clutter:ERROR:./clutter-actor.c:5759:clutter_actor_dispose: assertion failed: (priv->parent == NULL)``, 
caused by the code
  ``
  buttons.map(function (x) {
    x.destroy();
  });
  ``
