# Image Basics

### Overall Goal

To get familiar with libraries that mialab [depends on](https://github.com/ubern-mialab/mialab/blob/main/requirements.txt), so you know what the data types and functions/methods that you'll use for the next several weeks look like.&#x20;

Libraries here = [numpy](https://numpy.org), [simpleITK](https://simpleitk.org). Later on, you will also be friends with matplotlib, pillow and scikit-learn. Optionally, if you're very social and like even more friends, you could try nibabel, scikit-image and our homegrown kid, pymia.&#x20;

### Getting Started

This exercise is organized as a GitHub repository, where every time you commit a change, it automatically runs the test script and evaluates if you did the right thing or not. The code is here:

{% embed url="https://github.com/ubern-mialab/01-image-basics" %}

What you need to do next is to simply fork the repository, by logging into GitHub and then clicking on[https://github.com/ubern-mialab/01-image-basics/fork](https://github.com/ubern-mialab/01-image-basics/fork) so it creates a copy in your workspace.&#x20;

Then, you can simply open the script image\_basics.py ([https://github.com/ubern-mialab/01-image-basics/blob/main/image\_basics.py](https://github.com/ubern-mialab/01-image-basics/blob/main/image\_basics.py)) and then edit it, all within the browser: [https://github.com/ubern-mialab/01-image-basics/edit/main/image\_basics.py](https://github.com/ubern-mialab/01-image-basics/edit/main/image\_basics.py)

{% hint style="info" %}
Note that you'll have to change the location of the repository from \*/ubern-mialab/\* to \*/\<your-GitHub-username>/\* in the above links, once you have forked correctly.
{% endhint %}

If you think you've made the right changes to the file, feel free to then \*commit\* the change, using the green "commit changes..." button, and don't forget to include a helpful message about what the change really is.&#x20;

Then, wait for the cogwheels to run, GitHub runs it's 'actions' behind the scenes, and you'll either see a red ❌ or a green ✅ next to the commit message you entered previously.&#x20;

The goal really is to get the green ✅ every time you make a change, which will only happen when all the functions are completed correctly (correctly as defined by the tests in test\_image\_basics.py, please don't cheat ;-)). Clicking on the check mark will show more details about completion of the homework.&#x20;

Once you're done, please share a link to your fork with us, so we can confirm you've completed the assignment for the bonus grade (if such a need arises).

### Tasks and specifics

load\_image - load an image using the SimpleITK python interface, and return the pixel data based on if it is a label or not.

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L5](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L5)



to\_numpy\_array - transform the SimpleITK image to a numpy ndarray.

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L18](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L18)



to\_sitk\_image - transform the numpy ndarray to a SimpleITK image (the reverse of the previous function)

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L28](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L28)



preprocess\_rescale\_numpy - rescale the intensities of the np\_img to the range \[new\_min\_val, new\_max\_val].

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L42](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L42)



preprocess\_rescale\_sitk - rescale the intensities of the img to the range \[new\_min\_val, new\_max\_val], but this time, using SimpleITK

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L56](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L56)



register\_images - execute the registration\_method to the img (hint: fixed=atlas\_img, moving=img); see helpful comments within the function body here:  [https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L67](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L67)



extract\_feature\_median - apply median filter to image

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L93](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L93)



postprocess\_largest\_component - get the connected components from the image

[https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L103](https://github.com/ubern-mialab/01-image-basics/blob/d05df6945dee4841f7016cd2aab28a2eb800ffd7/image\_basics.py#L103)



### Help?

Numpy documentation: [https://numpy.org/doc/stable/user/absolute\_beginners.html](https://numpy.org/doc/stable/user/absolute\_beginners.html)

SimpleITK documentation: [https://simpleitk.readthedocs.io/en/master/gettingStarted.html#python-binary-files](https://simpleitk.readthedocs.io/en/master/gettingStarted.html#python-binary-files)&#x20;

If neither of these two help, reach out to the instructors on Slack. Responses are not guaranteed to be time bound, we will do our best.
