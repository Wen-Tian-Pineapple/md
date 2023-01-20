# SI 506: Problem Set 02

## This week's Problem Set

This week's problem set includes five problems (plus a bonus question) that focus on strings, lists,
and string/list operations.

:bulb: In order to check your work, try using the built-in function `print()` to print out the
results.

<br />

## Reference

- ["Python Built-in Functions"](https://www.w3schools.com/python/python_ref_functions.asp)
- ["Python Operators"](https://www.w3schools.com/python/python_operators.asp)
- ["Python List Methods"](https://www.w3schools.com/python/python_lists_methods.asp)
- ["Python String Methods"](https://www.w3schools.com/python/python_ref_string.asp)

<br />

## Background

The University of Michigan offers numerous resources that can help you and other students in their
well-being journeys. Below is a multiline string that provides a select group of U-M well-being
resources available to all students.

```python
wellbeing_resources = (
    "Dean of Students Office|734-764-7420, "
    "Sweetland Center for Writing|734-764-0429, "
    "Office of the Ombuds|734-763-3545, "
    "Counseling and Psychological Services (CAPS)|734-764-8312, "
    "Wolverine Wellness|, "
    "Sexual Assault Prevention and Awareness Center (SAPAC)|734-764-7771, "
    "Trotter Multicultural Center|734-763-3670, "
    "Spectrum Center|734-763-4186, "
    "Maize and Blue Cupboard (MBC)|734-936-2794, "
    "Ginsberg Center for Community Service Learning|734-763-3548"
)
```

We hope this assignment will increase your awareness of the numerous resources that UMich offers for
your benefit as listed in the SI 506 [Syllabus](https://si506.org/syllabus/).

:bulb: Learn more about U-M well-being resources by visiting
[https://wellbeing.studentlife.umich.edu/](https://wellbeing.studentlife.umich.edu/).

<br />

## 1.0 Problem 01 (30 Points)

**Task:** Create a master list of all wellbeing resources, then create sublists for different
categories of resources.

1. You have been provided with a variable containing a single string expressed across multiple lines
   named `wellbeing_resources`. Review each resource and note which character(s) delineate
   (separate) each resource. Call the appropriate string method to return a list of resource
   elements. Assign the return value of the string method to the variable `resources`, and display
   its contents.

2. Assign the first three elements of `resources` to a new list variable named `academic` using list
   slicing.

   :exclamation: You are limited to a single statement that includes a slicing expression.

3. Assign the fourth and fifth elements of `resources` to a new list variable named `health` using
   list slicing.

   :exclamation: You are limited to a single statement that includes a slicing expression.

4. Assign the sixth, seventh, and eighth elements of `resources` to a new list variable named
   `marginalized_comm` using list slicing and negative index values.

   :exclamation: You are limited to a single statement that slices the list using negative index
   values.

5. Assign the last two elements of `resources` to a new list variable named `community` using list
   slicing and negative indexing.

   :exclamation: You are limited to a single statement that slices the list using negative index
   values.

<br />

## 2.0 Problem 02 (30 Points)

**Task:** Update some of your resource sublists with additional resources using various list
methods.

1. Call the appropriate `list` method to extend `health` with `addl_health_resources`.

   :exclamation: The value assigned to `health` _must_ match the list below after calling the list
   method:

   ```python
   ['Counseling and Psychological Services (CAPS)|734-764-8312', 'Wolverine Wellness|', 'University Health Service (UHS)|734-764-8320', 'SilverCloud|734-936-8660']
   ```

2. Call the appropriate `list` method to add `embedded_caps` as the last `health` element.

3. Call the appropriate `list` method to insert `mesa` as the third `marginalized_comm` element.

4. Using list indexing and string concatenation, mutate `addl_academic_resources` by
   concatenating _each_ element with the respective phone numbers in `addl_academic_resource_numbers`.

   :exclamation: The value assigned to `addl_academic_resources` _must_ match the list below after concatenating
   the strings:

   ```python
   ['Office of Student Conflict Resolution|734-936-6308', 'Services for Students with Disabilities (SSD)|734-763-3000']
   ```

5. Call the appropriate `list` method to extend `academic` with `addl_academic_resources`.

   :exclamation: The value assigned to `academic` _must_ match the list below:

   ```python
   ['Dean of Students Office|734-764-7420', 'Sweetland Center for Writing|734-764-0429', 'Office of the Ombuds|734-763-3545', 'Office of Student Conflict Resolution|734-936-6308', 'Services for Students with Disabilities (SSD)|734-763-3000']
   ```

<br />

## 3.0 Problem 03 (15 Points)

**Task:** Resort some of your resource sublists using various list methods. Create an additional
list with resources from the health sublist.

1. Use the appropriate list method to _reverse_ the order of `marginalized_comm` elements.

2. Use the appropriate list method to sort the order of `health` elements in _ascending_
   alphanumeric order.

3. Use the appropriate list method to sort the order of `academic` elements in _descending_
   alphanumeric order.

   :bulb: Be sure to also specify the parameter `reverse` in the relevant list method
   as `True` `(reverse=True)`.

4. Using the appropriate list method, return the index value of
   `UMSI Embedded CAPS Psychologist|Ashley Evearitt` in `health`. Assign the index value to the
   variable `umsi_caps`.

5. Slice `health` using `umsi_caps` in your slicing expression. Slice
   `UMSI Embedded CAPS Psychologist|Ashley Evearitt` and
   `University Health Service (UHS)|734-764-8320` from `health`. Assign the new list to a variable
   named `student_focused_health_resources`.

   :exclamation: You are limited to a single statement that utilizes `umsi_caps` in your slicing
   expression.

<br />

## 4.0 Problem 04 (10 Points)

**Task:** Using the built-in functions `str.split()` and `str.join()` to create tuples and
variables.

1. Retrieve the third element from `academic` and convert it into a two-item tuple with the name as
   the first item and the phone number as the second. Assign this tuple to a variable named
   `third_academic_element`.

   :exclamation: Your output _must_ match the following:

   ```python
   ('Office of the Ombuds', '734-763-3545')
   ```

2. Retrieve the second to last element from `health` using _negative index values_ and convert it
   into a two-item tuple with the name as the first item and the phone number as the second. Assign
   the tuple to a variable named `second_last_health`.

   :exclamation: Your output _must_ match the following:

   ```python
   ('University Health Service (UHS)', '734-764-8320')
   ```

3. Working with `marginalized_comm`, call the appropriate string method that accepts an _iterable_
   (e.g., a list) as an argument and returns a new string composed of the `marginalized_comm`
   elements, each of which is separated by a period/fullstop (.). Assign the new string to a
   variable named `marginalized_comm_str`.

   :bulb: Your output _must_ match the following:

   ```python
   'Spectrum Center|734-763-4186.Multi-ethnic Student Affairs (MESA)|734-763-9044.Trotter Multicultural Center|734-763-3670.Sexual Assault Prevention and Awareness Center (SAPAC)|734-764-7771'
   ```

<br />

## 5.0 Problem 05 (10 Points)

**Task:** Create lists and find values using slicing.

1. Slice every odd-indexed value from `health` and assign the resulting list to a variable called `odd_index_health`.

2. Slice the 2nd, 3rd and 4th values in _reverse_ order from `academic` using **negative indexes**.
Assign the resulting list to a variable named `academic_sub_list`.

:bulb: Hint: Make sure to make sure of the `step` value within a list slice along with the `start`
and `stop` values.

   :exclamation: Your output _must_ match the following:

   ```python
   ['Office of Student Conflict Resolution|734-936-6308', 'Office of the Ombuds|734-763-3545', 'Services for Students with Disabilities (SSD)|734-763-3000']
   ```

3. Reverse the `marginalized_comm` list using negative indexes. Assign the resulting list in a
   variable called `marginalized_comm_reversed`.

   :exclamation: Your statement _must not_ use the `.reverse()` method.

<br />

## 6.0 OPTIONAL BONUS PROBLEM (10 points)

**Task:** Return a slice of `academic` using various list methods.

1. Use the appropriate list method to return the index of the last element in `academic`
   (i.e., `Dean of Students Office|734-764-7420`). Assign the value to a variable named
   `student_dean_index`.

   :exclamation: You _must_ employ the appropriate list method to retrieve the index value of this
   element.

2. Use `student_dean_index` in a slicing expression that slices two (`2`) elements from `academic`
   _in the following order_:

   1. `Dean of Students Office|734-764-7420`
   2. `Office of the Ombuds|734-763-3545`

   Assign the slice to a variable named `academic_sub_list.`

   :bulb: Your output _must_ match the following:

   ```python
   ['Dean of Students Office|734-764-7420', 'Office of the Ombuds|734-763-3545']
   ```
