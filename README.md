ML pipeline for predicting tags for stackoverflow questions


Architecture:
![architecture](https://github.com/AtufaShireen/aiops-dvc-nlp/blob/master/55AD9A79-EC2B-4201-8D39-7A6057970E0B_1_201_a.jpeg)
## STEPS -

### STAGE 01- Get Data
Extracting data from aws s3 bucket to required folder.


### STAGE 02- Prepare Data
1. Parsing the raw data(from xml tags).

### STAGE 03- Featurize
1. Featurize training features.
2. Featurize label feature into multilabel.
3. Featurizing the data into vector format.

### STEP 03- Train Model
1. Get preprocessed data.
2. Get params.
3. Train model.
4. Store model in artifacts.

### STAGE 04- Evaluate Model
1. Calculate metrics using model.
2. Add metrics to artifacts.


### DVC Utils
1. params.yaml: parameters for model.
2. config.yaml: configuration such as paths.
3. dvc.yaml: for creating pipeline.
4. setup.py: for packaging model.
5. artifacts: models, pipeline, featurizer, metrics.
