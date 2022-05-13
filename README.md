# vue-3-refs
Using Vue 3 refs in Vue -cli.

Here is the page render.  There are two components.

1.  A.vue a header component
2.  B.vue template containing 9 DIVS component

The 9 DIVS are simply a 50px square colored box, each defined by an HSL increment of n=36.
The idea is simply to expand a box by 1.25 times using a click event.

![image](https://user-images.githubusercontent.com/89032071/168347238-5461af05-816c-4e2b-8546-04b0628fbba3.png)

Here is the B.vue component (only).

![image](https://user-images.githubusercontent.com/89032071/168347641-ffa70698-32e5-4aa1-9bfe-b7b8897c4302.png)

The main purpose of this post is to 'refresh' how to use the refs in Vue.

1.  The ref on an element is used to capture the DOM object.
2.  ref="id=0" is the syntax within the <div> element; <div ref="id=0">, as the following screenshot red arrow indicates.
3.  console.log(this.$refs) will log the DOM object to the console.
4.  Now, you can use this.$refs for object refinement.

![image](https://user-images.githubusercontent.com/89032071/168346330-80203c06-0cf1-43c7-a86c-389a8f81200c.png)


