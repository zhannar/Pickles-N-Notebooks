# Pickles-N-Notebooks
These are functions which can be used to extract the input pickles that an IPYNB notebook might leverage, and all the output pickles it might ouput.

The **summerize_pickles()** function takes as an input the filepath to an .ipynb notebook file. The output is a dictionary with two keys: "input_pickles" & "ouput_pickles."

The "input_pickles" talls you what pickles the notebook reads into it and the "output_pickles" are those which are dumped to local memory.

If there are duplicate pickles in either list, that means the pickle was read in/dumped multiple times. That seems like a good thing to know in order to clean up... 