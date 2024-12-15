DSAIT4 - Project work

Instructors: Cynthia Liem and Annibale Panichella

For the assignment, you will work with (synthesized) data on risk modeling of citizens of Rotterdam. On Brightspace, under ‘Final Assignment’, you can find extensive documentation on the journalistic context of this particular use case and the model the Rotterdam municipality built on it.

The journalists performed bias audits on the Rotterdam model; both the original training code for the model and the journalists’ way of testing it are available under: https://github.com/Lighthouse-Reports/suspicion_machine

In our assignments, we will have you building your own models, implement your own testing techniques, and use them to audit your own and other groups’ models. To align better with the contexts in which you have been working as part of the labs, we decided to have you doing this in Python.

Part 1 - Training two models

Deadline - Week 5, December 13, noon.

In this first project assignment, you will train two machine learning models for the Rotterdam fraud prediction use case:

    A model that is purposefully bad;
    A model that is ‘as good as possible’.

In both cases, it should be possible to demonstrate how good or bad the model is through black-box testing. Here, we invite you as groups to define what you would consider ‘good’ or ‘bad’. For example, a purposefully bad model may have a discriminatory bias (which you may amplify, by training it on a more biased sample of the original dataset), whereas an ‘as good as possible’ model may have been designed for higher robustness through purposeful data augmentation.

To complete this assignment, you can choose any model you prefer (e.g., decision trees, random forests, neural network) as long as it is compatible with the onnx exchange framework. A Zip file is attached which contains a sample onnx setup to help you get familiar with this.

Please name and refer to both your models as model_1 and model_2, making a randomized choice (e.g. by a coin flip) on whether the good or bad model will be model_1.  

By December 13th, noon, please hand in the following deliverables on Brightspace:

    For both model_1 and model_2:

        Binary files of your two models named model_1.onnx and model_2.onnx, respectively;

        A zip file model_1.zip and model_2.zip, including:

            The training code used to train and export model_1.onnx  and model_2.onnx. Similarly to the original Rotterdam case, do not release your training data with this (which you may have adjusted, compared to the original *.csv released on Brightspace).

            A model_1.md and model_2.md file, with a small hint to the group that will be auditing your models, on one aspect this group should try to test (e.g. possible gender bias in the risk modeling).

        Make sure these files are anonymized, that is, that another team cannot easily infer which team you are, or obviously see which of the two models is the good or bad one.

    An accompanying report containing:

        An explanation of what constituted the ‘bad’ and ‘good’ model for your group, and the steps you took to create them. Please refer to your code/implementation for any work you coded and automated in this procedure [suggested length: 4-5 pages];

        An explanation of relevant tests to demonstrate how ‘bad’ or ‘good’ your models are, with reference to your code/implementation for any automated steps you took in implementing them, and a report of how well both models perform according to your implemented tests [suggested length: 4 pages];

        For each of the models, as well as your implemented categories of tests, a reflection on current strengths and weaknesses [suggested length: 2 pages].
