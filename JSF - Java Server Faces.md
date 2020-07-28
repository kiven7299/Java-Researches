## JSF - Java Server Faces

### Basic

1. What is it:

   - **JavaServer Faces** (JSF) is a MVC web framework that simplifies the construction of User Interfaces (UI) for server-based applications using reusable UI components in a page
   - component based framework
   - [Facelets technology](https://www.javatpoint.com/facelets): view handler technology for JavaServer Faces (JSF). 

2. Architecture

   Implements MVC architecture

   ![img](https://viblo.asia/uploads/9a736b76-1b3c-4442-bf08-863a6cc26b66.jpg)

3. Lifecycle: https://www.tutorialspoint.com/jsf/jsf_life_cycle.htm

   More on lifecycle is written in **Facelets's Lifecycle**



#### References

1. Quick guide: https://www.tutorialspoint.com/jsf/jsf_quick_guide.htm



### Facelets's Lifecycle: 

1. Lifecycle starts when a client makes a new request for a web page which is created using Facelets. JSF creates a new component tree or javax.faces.component.UIViewRoot and placed into the FacesContext.
2. View is ready to populate with components for rendering. The UIViewRoot if available is applied to the Facelets.
3. The newly built view is rendered back as a response to the client.
4. On rendering, the state of this view is stored for the next request. The state of input components and form data is stored.
5. The client may interact with the view and request another view from the JavaServer Faces application. At this time, the saved view is restored from the stored state.
6. The restored view is once again passed through the JavaServer Faces lifecycle, which eventually will either generate a new view or re-render the current view if there were no validation problems and no action was triggered.
7. If the same view is requested, the stored view is rendered once again.
8. If a new view is requested, the **Step 2** is continued.
9. New view is rendered back as a response to the client.

