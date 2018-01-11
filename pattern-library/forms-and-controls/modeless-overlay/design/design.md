# Modeless Overlay

![Image of Modeless Overlay Empty State Callout](img/modeless-overlay-empty-state-callout.png)


**Usage Scenario** The modeless overlay is a pattern that can be used as a replacement for a traditional modal. The modeless overlay can be used in scenarios in which a user may have to access secondary actions or information in order to complete a task. The information and actions on the modeless overlay are directly connected to the main underlying UI and allow the user to still interact with this underlying UI even with the modeless overlay.

**Animation** Whenever an anchored overlay panel is expanded or collapsed, there is a subtle sliding motion that accompanies it. The panel glides in and out of the side of the underlying UI that it is anchored to.

**Accessing the Overlay Panel** The user can access the overlay panel by creating a new object, editing a line of text, selecting an object, or other actions from an access point featured on the main underlying UI.

**Position of the Overlay**
- The initial position of the overlay panel should never cover any persistent navigational elements such as a top or side navigation bar.
- An anchored overlay may be attached to one side of the underlying UI (top, left, right, or bottom).
- A free-floating overlays should appear close to the action that invokes it.

**Use with Modals**
- A modeless overlay may be used with a modal overlay to provide help or other other actions contextual to the modal.
- As with a non-modal UI, the modal should still be accessible when the modeless overlay is on top.
- At desktop resolutions, the size of free-floating overlays does not need to be constrained by the size of the modal. In other words, portions of the modeless overlay may hang over the darkened background around the modal.
- The modeless overlay may be moved anywhere on the viewport, including the darkened background.  
- If the width of a modeless overlay exceeds that of the modal, the content of the modeless overlay should replace the content of the modal, with a back button to return to the modal contents. This behavior is similar to the [mobile behavior](#modeless-overlay-mobile).   
- Dismissing the modal will also close the modeless overlay, as it is contextual to the modal.


**Other Details**
1. **Shadow:** There is a slight shadow around the overlay panel that helps to reinforce that it is located on top of the main page.  

2. **Close Button:** The close button allows the user to dismiss the overlay pattern. When the panel is closed, there is a slight animation that shows the overlay panel sliding back into the side it was anchored on.

3. **Title Area:** The primary name of the selected object helps to identify what is being shown on the panel and is featured at the top of the panel.

4. **Content Area:** Object specific content such as descriptive title, date, status, product owner, collaborators, description, etc. could live here.

5. **Optional View Full Page:** For applications that require it, a user may view the details featured on the panel in a larger environment by expanding the panel to be a full page. Once the full page has been activated, the user can get back to the standard view of the overlay panel by clicking on a button entitled "View Standard Page". This will return the modeless overlay back to its original state. The full-page view should not be used when the overlay is invoked from a modal.

![Image of Modeless Overlay Panel](img/modeless-overlay-panel-callout.png)

1. **Content Body:** The overlay panel may be used with a variety of different views such as list, table, or card view. When using the overlay panel in different types of content views, the user still has the ability to interact with the page underneath of the panel and can adjust the content of the panel by selecting a different object from the underlying page.

**Page Behavior:**

Vertical Navigation: If the content of the panel extends past the initial frame of the window a vertical scrollbar should be enabled.

Horizontal Scrollbar: In the case of the modeless overlay panel, a horizontal scrollbar should not be used.  

# Modeless Overlay- Mobile

![Image of Modeless Overlay Mobile](img/modeless-overlay-mobile-callout.png)

**Overlay Panel Behavior:** On mobile, the overlay panel would extend out to be full screen. The overlay panel should act as an extension of the underlying UI. It presents more detailed information about an object that was featured in the underlying UI. When the overlay panel is open, it should be the only element that the user can interact with. In order to access the underlying UI, the user must exit the overlay panel.

1. **Accessing the Overlay Panel:** On mobile, the user can access the overlay panel by creating a new object, editing a line of text, selecting an object, or other actions from the main underlying UI.

2. **Object Specific Content:** Within each object, the user can input and attach object specific content.

3. **Selecting Object Content:** When the underlying UI is populated with object content, the user can select an individual object and open the overlay panel that way. The overlay panel will show information regarding the selected object.

4. **Object Content:** The user can view general object information from the overlay panel.
