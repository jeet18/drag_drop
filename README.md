# drag_drop

#In this html you see drag and drop of an image from one div to another.

# Funstion used inside for drag and drop.
#function allowDrop(ev) {
  ev.preventDefault();
}

#function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}

#function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
