# Customizing fields 
While Blockly provides many useful fields, your application may have a specialized case. Here are a few steps to take when customizing fields:

  1. Read the documentation of any fields similar to what you require; they may provide a useful interface for customization. For example, [dropdowns](/guides/create-custom-blocks/fields/built-in-fields/dropdown) have a lot of hidden functionality.

  2. Consider using a [validator](/guides/create-custom-blocks/fields/validators) to solve your problem. Validators allow you to only accept certain values, modify input, or trigger functionality when a field's value changes.

  3. Consider [extending a field](/guides/create-custom-blocks/fields/customizing-fields/extending). If there is a field that represents the value type you require, but you want to modify its [editor](/guides/create-custom-blocks/fields/anatomy-of-a-field.html#编辑器显示), its [appearance](/guides/create-custom-blocks/fields/anatomy-of-a-field.html#块上显示), or the [text](/guides/create-custom-blocks/fields/customizing-fields/creating#text) it displays, you can [create a subclass](/guides/create-custom-blocks/fields/customizing-fields/extending#subclassing) that inherits the bulk of the functionality, while overriding the specific parts you want to change.

  4. [Create a new field type](/guides/create-custom-blocks/fields/customizing-fields/creating). While this is the most powerful option, it is also the most time consuming, and should generally only be used if you need to store a new value type.