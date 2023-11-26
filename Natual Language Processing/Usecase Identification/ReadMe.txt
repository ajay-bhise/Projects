

# Problem Statement  -

    From a given text we have to find the usecases or applications mentioned for given topic.

# example -

    * text - Primary (single-use or "disposable") batteries are used once and discarded, as the electrode materials are
           irreversibly changed during discharge; a common example is the alkaline battery used for flashlights and a
           multitude of portable electronic devices. Secondary (rechargeable) batteries can be discharged and recharged
           multiple times using an applied electric current; the original composition of the electrodes can be restored
           by reverse current. Examples include the lead–acid batteries used in vehicles and lithium-ion batteries used
           for portable electronics such as laptops and mobile phones.

    * usecases - ['flashlights','portable electronic devices','vehicles','laptops','mobile phones']

# Solution -

    * Approach 1 -

            I have tried to train a custom ner model using spacy-trf. This approach has better f1-score amongst all
            other open source models that iI have tried. This is because of the number of parameters and vocab size of
            this model.

    * Approach 2 -

            In this approach, I tried fine-tuning Opan AI's GPT-3-davinci model. I had design the prompt for the better
            output. This was costly. I had to spend $9.00 for training the same model with training data set size of
            500 records. This model gave better results than spacy-trf-custom-ner.