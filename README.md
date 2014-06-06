Gnome-Shell-Panel-World-Clock
=============================

Unofficial fork of https://extensions.gnome.org/extension/697/panel-world-clock/ -- Disclaimer: I am NOT the author, but I could not find anywhere the author has this hosted, and I wanted to make a change. Master will represent the version released on extensions.gnome.org. I will keep my changes in branches.


fixed for gnome-shell 3.10

### todo
  * due to following error:
  
  ``
  Clutter:ERROR:./clutter-actor.c:5759:clutter_actor_dispose: assertion failed: (priv->parent == NULL)
  is caused by the code below
  ``
  I've disabled the destruction of the buttons
  
  ``
  buttons.map(function (x) {
    x.destroy();
  });
  ``
