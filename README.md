# desmos-3d-export-obj

# installation 
drag this link to ur bookmarks bar -> [Desmos 3D Export](javascript:void%20function(){var%20a=Math.hypot;chunks=(b,a)=%3EArray.from(Array(Math.ceil(b.length/a)),(c,d)=%3Eb.slice(d*a,d*a+a));let%20b=(b,c)=%3Ea(b[0]-c[0],b[1]-c[1],b[2]-c[2]),c=[],d=[],e={},f=0;for(let%20a,d=0;d%3CObject.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces).length;d++){if(a=Object.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces)[d],root=a.mesh.geometry,4==root.attributes.position.array.length/3)continue;let%20g=chunks([...root.attributes.position.array],3);c.push(...g),g.forEach((a,d)=%3E{c.forEach((c,g)=%3E{d+f==g||.01%3Eb(a,c)%26%26(e[d+f]=g)})}),f+=Object.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces)[d]%3F.mesh.geometry.attributes.position.array.length/3}let%20g=0;for(let%20a,b=0;b%3CObject.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces).length;b++){if(a=Object.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces)[b],root=a.mesh.geometry,4==root.attributes.position.array.length/3)continue;let%20c=chunks([...root.index.array],3).map(a=%3Ea.map(a=%3E{return%20e[a+g]%3Fe[a+g]:a+g}).map(a=%3Ea+1));d.push(...c),g+=Object.values(Calc._calc.view.controller.grapher3d.webglLayer.surfaces)[b]%3F.mesh.geometry.attributes.position.array.length/3}let%20h=``;h+=c.map(a=%3E%22v%20%22+a.join(%22%20%22)).join(%22\n%22),h+=%22\n%22,h+=d.map(a=%3E%22f%20%22+a.join(%22%20%22)).join(%22\n%22),h+=%22\n%22,function(a,b){var%20c=document.createElement(%22a%22);c.setAttribute(%22href%22,%22data:text/plain;charset=utf-8,%22+encodeURIComponent(b)),c.setAttribute(%22download%22,a),c.style.display=%22none%22,document.body.appendChild(c),c.click(),document.body.removeChild(c)}(%22desmos-graph.obj%22,h)}();)

# usage
open desmos 3d graph, hide things that arent ur 3d volumes (so hide lines)
it doesnt export flat inequalities only 3d things
Once you have the file it gives you, put the obj file into some obj to stl converter, i used [this one](https://anyconv.com/obj-to-stl-converter/)
that will fix all the weird errors my code causes
youll get an STL and thats it! u did it! i love you! <333 
have fun :)
