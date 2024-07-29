!Creating html dynamically: lists of links
 let element_list = document.getElementById('list');
let new_li = document.createElement('li');
let new_a = document.createElement('a');
new_a.innerText = 'Rutracker  - biggest Russian torrent-tracker';
new_a.style.color = '#ff0000';
new_a.setAttribute("href", 'https://rutracker.org/forum/index.php');

new_li.appendChild(new_a);

element_list.appendChild(new_li);
let new_li2 = document.createElement('li');
let new_a2 = document.createElement('a');
new_a2.innerText = ' RadioRecord - great online-radio';
new_a2.style.color = '#ff0000';
new_a2.setAttribute("href", 'https://www.radiorecord.ru/?ysclid=lz79hdpqvt86465370');

new_li2.appendChild(new_a2);

element_list.appendChild(new_li2);
let new_li3 = document.createElement('li');
let new_a3 = document.createElement('a');
new_a3.innerText = 'CIA Uncensored files - a lot of interesting stories.';
new_a3.style.color = '#ff0000';
new_a3.setAttribute("href", 'https://www.cia.gov/readingroom/');

new_li3.appendChild(new_a3);

element_list.appendChild(new_li3);
element_list.style.backgroundColor = '#cccccc';
*****************************************************************************************************
!Buttons and clicks: A button to add apples
document.getElementById('button').addEventListener('click', (event) => {
  let element_list = document.getElementById('list');
  let new_li = document.createElement('li');
  new_li.innerText = 'apple';
  new_li.style.color = '#ff0000';

  element_list.appendChild(new_li);

});

document.getElementById('remover').addEventListener('click', (event) => {
  let element_list2 = document.getElementById('list');
  element_list2.replaceChildren();

});
!!!!!!!!!! html: 
<ul id="list"></ul>
<button id="button">add an apple</button>
<button id="remover">remove an apple</button>
******************************************************************************************************************************************
