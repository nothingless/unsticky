# unsticky
A bookmarklet that removes sticky elements:

javascript:(function () {var i, elements = document.querySelectorAll('body *');for (i = 0; i < elements.length; i++) {if (["sticky","fixed"].indexOf(getComputedStyle(elements[i]).position)>-1) { elements[i].parentNode.removeChild(elements[i]);}document.body.style.overflow="auto"; }})();
