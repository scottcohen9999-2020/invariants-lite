# invariants-lite
lightweight invariants for image recognition

# Table of Contents
- All configuration parameters
- Get the similarity vector, the object under investigation
- Is accuracy a useful metric i.e. are the class sizes balanced?
- Train to recognize the dataset and return all similarity vectors
- Test recognizing the dataset and return all similarity vectors
- Get accuracy of kNN and of similarity vector in conjunction with kNN
- Verbatim from Deep Learning with Python...
...by Francois Chollet, 2018 (page 120-122) including the hardcoded constants.

- Chop-up verbatim_from_book_CNN_orig() into reusable pieces
- Transformations for a percentage of all images
Use the above chopped up pieces from verbatim_from_book_CNN_orig()
Also, do StratifiedKFold() and do_transforms()
- Get StratifiedKFold accuracy of similarity vector in conjunction with verbatim_from_book_CNN
- End of function defs; start of using them
- Get two baselines: (1) verbatim_from_book_CNN; (2) random numbers
- Baseline (1): Get 5 reps of 10-fold StratifiedKFold accuracy of verbatim_from_book_CNN
- Each test is repeated for a dataset sizes of 12, 24, 36, 48, 60 thousand images
- Get baseline (1) where a percentage of the train and test is shrunk and in the upper left corner of picture
- Baseline (2): Get StratifiedKFold accuracy of appending rand #s
- Append both random numbers and similarity_vector together
- StratifiedKFold accuracy of test_CNN_with_similarity_vector TYPE=1
- Accuracy of 5 reps of 10-fold cross-validation, TYPE=-4
- Does accuracy improvement help the most with fewer images?
- Some Config choice tuning: type of similarity vector
- Comparison summary of accuracy of 5 reps of 10-fold cross-validation
- Some Config choice tuning: NUM_SPHERES aka donuts or shells
- Configuration: NUM_POWER_SUMS
- Areas for further work
- Phase 2 Other models: kNN, XGBOOST
