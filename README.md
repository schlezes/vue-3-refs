# vue-3-refs
Using Vue 3 refs in Vue -cli.

Here is a simple page render.  There are two components. These are single file components.

1.  A.vue a header component
2.  B.vue component containing 9 DIVS

The 9 DIVS are simply a 50px square colored box, each defined by an HSL increment of n=36.
The idea is simply to expand a box by 1.25 times using a click event.

![image](https://user-images.githubusercontent.com/89032071/168347238-5461af05-816c-4e2b-8546-04b0628fbba3.png)

Here is the B.vue component (only).

![image](https://user-images.githubusercontent.com/89032071/168347641-ffa70698-32e5-4aa1-9bfe-b7b8897c4302.png)

The main purpose of this post is to 'refresh' how to use the refs in Vue. 

Ref is a Vue special attribute. This attribute allows direct access to a specific DOM element.

1.  use "ref" (singular) syntax as keyword for the element that you want access to: ie, ref="id=0"

2.  use this.$refs to obtain the $refs element target.

3.  console.log(this.$refs) will log to the console the specific DOM element.

Explained another way,

1.  The ref on an element is used to identify the element object property in the DOM.
2.  ref="id=0" is the syntax within the <div> element. ref="id=0", as the following screenshot red arrow indicates.
3.  console.log(this.$refs) will log the DOM element object to the console.
4.  Now, you can use this.$refs for the target property object refinement.
5.  Use Reflect.get(this.$refs, 'id=0') to return the element object as a choice.
  
![image](https://user-images.githubusercontent.com/89032071/168395846-bf5beb91-c80e-4c66-ab78-97542bab3ab6.png)

And now, the Vue Dev Tools screenshot.
  
  ![image](https://user-images.githubusercontent.com/89032071/168374821-cfd424b7-7561-44fc-93b4-bd1acccae30f.png)

