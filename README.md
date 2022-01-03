# ***Neural Network Charity Analysis***

## **Purpose:**
By using neural networks we analyzed over 34,000 organizations that recieved funds from different charities. Through this analysis we wanted to see if these applicants will be successful if they were to be funded by Alphabet Soup. 

## **Results:**
### Data Preprocessing
- Target variable was the column IS_SUCCESSFUL. The EIN and NAME columns were dropped.
- Features included: application type, affliation, classification, use_case, organization, status, income_amt, special_considerations, and ask_amt.

### Compiling, Training, and Evaluating the Model
We started with 110 initial neurons that were spread over two hidden layers that had 80 in the first and 30 in the second. The activation function that we used was ReLu in the hidden layers and for the outer layer the Sigmoid activation function was used. 
Unfortunately we didn't reach the 75% accuracy neither in the initial attempt nor in the other 3 attempts that were optimized. The optimization that we implemented were increasing the number of hidden layers up to 4 while also increasing the nuerons in each layer. Additionally, we changed the activation function to tanh and LeakyReLU.

## **Summary:**
In conclusion, using this model we were unable to achieve the 75% accuracy requirement. The accuracy score was close at 72% but not enough. A different model that can be used for this dataset might be the random forest model since it might be better at identifying the more important features for the outcome. 