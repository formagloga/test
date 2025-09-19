# test
# Système de composant dans EtchWP

Voici la documentation d'Etch sur les composants


Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsIntroduction to Components

Components in Etch

Components are the fundamental building blocks of modern web development. They are reusable, self-contained elements or groups of elements that can be combined to create complex layouts and functionality.

Each component is a self-contained chunk of code that handles a specific part of your website’s look or functionality, and you can use it many times across different pages and areas of your site. It can render the same content over and over again, or each instance can render unique content.

Here are some examples of common components:

Header: The top bar with your logo, navigation (Shop, About, Contact), and perhaps a CTA. It's built once and reused on every page for consistent navigation.

Footer: The bottom section with contact info, social media links, and perhaps a newsletter signup.

Cards: Product displays showing a product's image, name, and price. You reuse the same card design for every product on your site, perhaps with different variations or attributes.

Call to Action Areas (CTAs): Promotional banners with special offers, discount codes, or limited-time deals. These components can be reused across your site to highlight sales, new products, or seasonal promotions.

Buttons: Interactive elements that trigger actions like form submissions, navigation, or data processing. These components can be customized with different styles, sizes, and behaviors while maintaining consistent design patterns across your site.
info

Many traditional builders refer to components (like the header and footer, but even other types of components) as "templates." This is incorrect & confusing nomenclature and is an architectural disaster. Components and templates are two very different things. If you come from the world of page building, it's important to retrain your brain to understand components separately from templates.
Why components are useful

    Reusability: Create a component once and use it throughout your site. A card component, for example, can be used for products, services, or blog post previews with different content and styling.

    Consistency: Components ensure consistent design and behavior across your site. When you update a component, all instances automatically reflect the changes.

    Maintainability: Breaking your UI into components makes your project more organized and easier to maintain because each important part of your site has a single source of truth.

    Scalability: Components make it easy to add new features or pages by combining existing components in new ways.

How components handle data

Props control how each instance of a component renders and behaves and the unique content that's passed into key areas of your component.

For example, if you have a card for displaying information for a service, you wouldn't want every card to repeat the same service name. The only way a component is useful is if each component instance can display a different service.

To make this work, you create a "prop" (property) for the name of the service, like serviceName, and then you plug that prop into the heading area of the card. Now, when you add a service card component, you fill out the field for service-name and the component will display the correct service name.

A text prop like this is essentially a placeholder for whatever text content you want to add.

We'll talk more about data props later.
How components can have variations

Props also allow you to control how a component behaves.

For example, let's say you're creating a card component for e-commerce products. You want to make sure that when a product is on sale, you can display an "on sale" badge.

You can create a boolean prop (there are many different prop types to help you accomplish your goals) called onSale. Boolean props resolve to true or false. You can then create your "on sale" badge and place it inside a conditional logic element in Etch. This conditional logic element can check the value of onSale and show the badge if it's true and hide it if it's false.

We'll talk more about boolean props and component variants later.
Conclusion

Whether you're building a simple landing page or a complex e-commerce site, components will help you organize your code, maintain consistency, and deliver a better developer experience. The reusability and maintainability that components offer make them an essential tool in any web developer's toolkit.
Next steps

Now that you understand the basics of components, here are the next steps to continue your learning journey:
Last updated on Sep 18, 2025
Previous
Content Slot
Next
Creating a Component

    Why components are useful
    How components handle data
    How components can have variations
    Conclusion
    Next steps

Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.


Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsCreating a Component

Creating a Component

Ready to create your first component in Etch? It's super easy!
1. Create a static version of your component

Before you actually create a component, you should build the thing that you'll eventually turn into a component. For example, if you're going to build a header component, just build a header first. You can make it a component when you're done.

Building a static version of the component is the easiest and quickest way to create new components.
2. Click "Create Component"

Once your static version is ready, right click it in the structure panel (whatever the parent element is) and choose "Create Component" from the context menu.

This will take you into the component editor. You'll know you're in the component editor because everything will be purple and you'll see the "Component Editor" panel in the interface (though it won't have any props yet).

Component Editor Interface
3. Name Your Component

If you named the parent element in the structure panel (like the fantastic developer you are) then the component will already be named exactly what you wanted it to be named.

If you didn't name your structure panel elements (shame!), then you can double click the component label and edit it.
4. Create your props (if needed)

Not all components need props. If your component doesn't need props, skip to the next step. If it does, reference Creating Component Props.
5. Save your component

Your component is not a component until you hit the purple "Save" button at the bottom right of the interface when in the component editor.

Once you've saved your component, you can then hit the "Exit" button. If you hit "Exit" before saving, you'll abandon the component creation process (helpful if you change your mind about creating a component).

The reason "Save" doesn't close the component editor is because it's common to want to save progress when building a component without being evicted from the component editor. If you want or need to exit, just click "Exit."
Component Best Practices

    Use descriptive names: Choose names that clearly indicate what the component is or does
    Keep components focused: Each component should have a single, clear purpose
    Make components maintainable: Components should have logical structures and maintainable styling (e.g. BEM and variable-first CSS)
    Make components flexible: Design components to work in different contexts
    Use props for customization: Instead of hardcoding values, use props to make components dynamic

Next Steps

Once you've created a component, you can:

    Add component props
    Map component props
    Use a component on pages
    Use a component in templates or loops
    Create component variations

Last updated on Sep 18, 2025
Previous
Introduction to Components
Next
Creating Component Props

    1. Create a static version of your component
    2. Click "Create Component"
    3. Name Your Component
    4. Create your props (if needed)
    5. Save your component
    Component Best Practices
    Next Steps

Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsCreating Component Props

Creating Component Props

Props are the customizable properties that make components dynamic and reusable. They allow you to pass different data and control how components behave in different contexts.

Think of props as the "settings" for your component. Just like how you can adjust the settings on your phone (brightness, volume, etc.), props let you adjust how your component looks and behaves and what it says.
Prop Planning

There are two main types of props:
1. Data Props

Data props are placeholders for content that changes between component instances. They allow you to display different information while maintaining the same structure and styling.

Examples of data props:

    Text content: Titles, descriptions, labels
    Images: Featured images, logos, icons
    Links: URLs for buttons, navigation items
    Numbers: Prices, ratings, quantities

Example scenario: A product card component might have data props for:

    productName - The name of the product
    productPrice - The price of the product
    productImage - The product's image
    productDescription - A brief description

2. Behavior Props

Behavior props control how a component functions or appears. They typically use boolean values (true/false) or specific options to determine component behavior.

Examples of behavior props:

    Visibility controls: Show/hide elements based on conditions
    Style variations: Different visual states (active, disabled, featured)
    Functionality toggles: Enable/disable features
    Layout options: Different arrangements or sizes

Example scenario: A button component might have behavior props for:

    isDisabled - Whether the button is clickable
    isPrimary - Whether to use primary or secondary styling
    size - Small, medium, or large button size
    showIcon - Whether to display an icon alongside text

Why Props Matter

Props make your components:

    Reusable: Use the same component with different content
    Flexible: Adapt to different contexts and requirements
    Maintainable: Update one component to affect all instances
    Consistent: Maintain design standards across your site

Adding Props in Etch

To add a prop to a component, click the "+" icon near the top of the component editor panel.

Adding a prop to a component

Next, click on the prop type that you're wanting:
Available Props

    Text - A simple text input for titles, descriptions, labels, or any string content.
    Boolean - True/false values for controlling visibility, states, or conditional behavior.
    Select - Dropdown options for choosing from predefined values (like sizes, categories, or themes).
    Image - Image upload and selection for photos, icons, logos, or any visual content.
    Array - Multiple values or objects for lists, collections, or complex data structures.
    Slot - Content areas where you can drag and drop other components or elements.

Once added, you'll see it in the Component Editor.

Adding a new prop to a component

Every prop has two mandatory values: Name & Key

    Label - The display name that appears in the component editor interface
    Key - The internal identifier used in code and data mapping

You can double click the Label to edit and the same is true for Key.

Repeat the process for all necessary props.
Next Steps

Now that you understand the basics of adding props, the next step is:

    Map props to your component

Last updated on Sep 18, 2025
Previous
Creating a Component
Next
Mapping Component Props

    Prop Planning
        1. Data Props
        2. Behavior Props
    Why Props Matter
    Adding Props in Etch
        Available Props
    Next Steps

Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsText Prop

Text Prop

The text prop is the most basic component prop. It allows you to dynamically insert a string of text into a component. It should be used whenever a text string or "textarea" is needed.
Last updated on Sep 18, 2025
Previous
Creating Component Variations
Next
Boolean Prop
Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsBoolean Prop

Boolean Prop

The Boolean Prop is a true/false toggle switch. It's typically used for conditional logic, or for on/off styling via attributes or container style queries.
Last updated on Sep 18, 2025
Previous
Text Prop
Next
Select Prop
Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsSelect Prop

Select Prop

The Select Prop is a dropdown selection field that allows you to declare multiple key : value pairs with the "key" essentially being the "label" or "option" in the dropdown. The "value" is typically output as code.

If the key and value are to be the same, you can define a single key, which will also be the value by default.

One key, or one key-value pair, should be placed on each line.
info

When writing a key/value pair, it's imperative that you put a space between the key (label), the ":" (separator), and the value when defining key/value pairs.

Incorrect: key:value

Correct: key : value.

Referencing a select prop with dynamic data will output the value of the prop by default. It's not currently possible to output the key, though it will be in the future.
Last updated on Sep 18, 2025
Previous
Boolean Prop
Next
Image Prop
Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsImage Prop

Image Prop

The Image Prop allows you to reference an image file from the media library or any image URL.
note

The image prop does not automatically pull any alt value from the media library. For full image support, it's best to create an image prop and then a text prop for the image's alt tag.
warning

The image prop does not currently support srcset, but will in the future.
Last updated on Sep 18, 2025
Previous
Select Prop
Next
Loop Prop
Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsLoop Prop

Loop Prop

The Loop Prop creates an internal loop reference. It's useful for when you're including a loop inside your component and need to be able to choose the Loop Source when adding your component to a page.

Since components might be used on multiple sites, or with different loops at different times, you might want to build a loopable structure inside your component without creating a fixed reference to any specific loop. The Loop Prop allows you to select the loop that should run inside the component when you're using the component.

Here's the difference between a typical loop and a prop-based loop:
Typical Loop

{#loop some-loop as item}{/loop}

Prop-Based Loop

{#loop props.your-loop-prop as item}{/loop}

info

Props are typically referenced with {} brackets. However, when you're already working within bracketed data, you should not use another set of brackets.

Incorrect: {#loop {props.your-loop-prop} as item}{/loop}

Correct: {#loop props.your-loop-prop as item}{/loop}
Last updated on Sep 18, 2025
Previous
Image Prop
Next
Component Slots

    Typical Loop
    Prop-Based Loop

Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
Skip to main content
Etch Logo
Documentation
Purchase

    Etch Documentation
    Getting Started
    Interface
    Elements
    Templates
    Components
        Introduction to Components
        Creating a Component
        Creating Component Props
        Mapping Component Props
        Using a Component (Static)
        Using a Component (Dynamic)
        Creating Component Variations
        Component Props
            Text Prop
            Boolean Prop
            Select Prop
            Image Prop
            Loop Prop
            Component Slots
    Dynamic Data
    Loops
    Conditional Logic
    Responsive Development
    Utilities
    Gutenberg
    How To
    Integrations

    Known Issues
    Current Priorities
    Feature Flags

    ComponentsComponent PropsComponent Slots

Component Slots

A Slot in a component is not actually a "prop" the way other props are. You can think of a Slot as a "drop zone" that can accept any content. It allows you to place anything inside a component from the outside.

Slots can be difficult to wrap your head around at first. The best way to think about it is this:

Every other "prop" in component design forces you to define exactly what type of data is accounted for and/or allowed: text, image, boolean, link, etc.

Slots, on the other hand, let you define an area of the component where anything can be dropped in.

The easiest example to understand is an accordion component for Frequently Asked Questions.

The accordion heading is almost always just text, so you can easily use a text prop. This will allow us to write the "question" part of the FAQ.

What about the content of the accordion, though — the answer part of the FAQ?

Should it be text? Should it be a combination of text and images? How much text? How many images? What if I want to include a link? What if I want to include a button? How do we determine what style of button?

That's a lot of questions. And if we have to configure props and conditional logic for all the possibilities, that's going to be a tremendously complex component that still ends up with a lot of limitations.

Instead of programming all that complexity via props, all we have to do is define a slot in the accordion content area. Once the slot is defined, users can drop anything they want in the slot and be happy. 100% flexibility with zero complexity!

To add a slot, click the slot icon and give it a name in camelCase. Make sure you place the slot in the area of the component where you want slot content to show up. That's it!
Last updated on Sep 18, 2025
Previous
Loop Prop
Next
Dynamic Data Intro
Copyright © 2025 Digital Gravy. Etch™ is a Trademark of Digital Gravy.
