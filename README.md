# Cancer_Daigonosis
Finding actionable genetic mutations that causes cancer using Machine Learning
<table style="width:70%">
  <tr>
    <th>Algorithm</th>  
    <th>Model</th>
    <th>Percent of misclassified point</th> 
    <th>Dimension</th>
    <th>Test Logloss</th>
  </tr>
  <tr>
    <td> SGDClassifier with log loss </td>
    <td>OneHotEncoded Gene, Variation + 1gram TFIDF + 1,2gram CountVectorizer of text</td>
    <td>NA</td> 
    <td>785767</td>
    <td>1.1492</td>
  </tr>
    
  <tr>
    <td> Logistic Regression Fine tuned </td>
    <td>Same as model 1</td>
    <td>35.187%</td> 
    <td>785767</td>
    <td>1.0912</td>
  </tr>
  
   <tr>
    <td> Logistic Regression Fine Tuned </td>
    <td>OneHotEncoding of Gene, Variation, 1,2,3gram TFIDF of 20000 features </td>
    <td>30.075%</td> 
    <td>22182</td>
    <td>0.8864</td>
  </tr>
  
  <tr>
    <td> Fine tuned Logistic Regression + Fine tuned RandomForest </td>
    <td>Manual average ensemble of model2 + fine tuned RandomForest of 
        response coding of gene, variation, text + binary countvectorizer
        of text.
    </td>
    <td>29.924%</td> 
    <td>NA</td>
    <td>0.8736</td>
  </tr>
  
</table>

