# homework #2
 
## Instructions

1. Use the [**COVID Image Classification Hackathon** competition](https://www.modelshare.org/detail/model:1539) created for this homework. In particular, rely on the instructions and starter code in the [**COVID image classification starter code** notebook](https://www.modelshare.org/notebooks/notebook:340) to load the correct train and tests sets, and to submit your model.
2.Write a report in a Jupyter notebook and `push` it to your homework repo. When you are done with your homework **submit the link to this GitHub repo through Courseworks**.

---

Your report should include the following information [`100 pts`]:

* [`10 pts`] **Citation of paper providing original dataset:**  M.E.H. Chowdhury, T. Rahman, A. Khandakar, R. Mazhar, M.A. Kadir, Z.B. Mahbub, K.R. Islam, M.S. Khan, A. Iqbal, N. Al-Emadi, M.B.I. Reaz, “Can AI help in screening Viral and COVID-19 pneumonia?” arXiv preprint, 29 March 2020, https://arxiv.org/abs/2003.13145
* [`10 pts`] Visualize images that demonstrate when x-rays demonstrate Covid Postivity and when they do not (You can present visuals of each category in the data if you would like to.).
* [`10 pts`] Discuss the dataset in general terms and describe why building a predictive model using this data might be practically useful.  Who could benefit from a model like this? Explain.
* [`20 pts`] Run at least three prediction models to try to predict x-ray images well. Use transfer learning for at least one of these models
* [`10 pts`] Discuss which models performed better and point out relevant hyper-parameter values for successful models.
* [`20 pts`] Submit your best model to the leader board for the [**COVID Image Classification Hackathon** competition](https://www.modelshare.org/detail/model:1539).
* [`20 pts`] Import the best model from the leader board (whatever the best model is after your final submission)
Note:
	* Use the `aimodelshare` `instantiate_model()` function
	* Visualize the model's structure using `tf.keras` `model.summary()`
	* Explain how the model's structure is different from your best model.
	* Explain how the model's optimization approach is different from your best model
	* Fit the best model from the leader board to training data and evaluate it on test data to complete your report.
