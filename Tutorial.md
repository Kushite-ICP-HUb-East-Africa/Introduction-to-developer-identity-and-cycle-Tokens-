# Create a Developer Identity, Claim Cycle Tokens, and Deploy a Simple Canister on IC

1. **Apply for Free Cycles from a Cycles Faucet:**
    - Obtain a coupon code for redeeming cycles from a [cycles faucet](https://anv4y-qiaaa-aaaal-qaqxq-cai.ic0.app/). In the survey, enter `0TOICP` as the name of your project. After receiving your coupon, you can then move on to the steps below.
        
        ![Screenshot from 2023-11-27 16-28-43.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c449c26a-1935-47bd-809e-51dbfecd9cca/2cac72ff-70f6-4a7b-96a8-a7e7ced11096/Screenshot_from_2023-11-27_16-28-43.png)
        
2. **Create a New Developer Identity**:
    - Open a terminal on your computer.
    - Create a new identity using the **`dfx`** command:
        
        ```
        dfx identity new <identity_name>
        ```
        
        - This is for development and deployment purposes. It allows you to manage multiple profiles when interacting with your local development environment or the Internet Computer network.
    - Set this identity as the default:
        
        ```
        dfx identity use <identity_name>
        ```
        
    - Display a list of all identities you have created, including the default identity.
        
        ```
        dfx identity list
        ```
        
    - **Take a screenshot** of the terminal window showing the results. Make sure that only the relevant information (the list of identities and the default one) is visible in the screenshot.
    - ***Important**: Be cautious not to include your seed phrase in the screenshot. The seed phrase should be kept private and secure at all times.*
        
        ![Screenshot from 2024-02-08 03-49-29.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c449c26a-1935-47bd-809e-51dbfecd9cca/e671cf7f-d156-4804-8572-3ec4063a75f3/Screenshot_from_2024-02-08_03-49-29.png)
        
3.  **Claim Cycles with Redeem-Faucet-Coupon and Check Your Balance**:
    - Use the coupon you obtained to redeem your free cycles.
        
        ```
        dfx wallet --ic redeem-faucet-coupon <your coupon-code>
        ```
        
        - This step involves creating a cycles wallet by redeeming free cycles, instead of the usual method of converting ICP tokens.
            
            ![Screenshot from 2024-02-08 04-06-04.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c449c26a-1935-47bd-809e-51dbfecd9cca/2a3749d8-d875-411e-a5c9-1ebb603b9ddc/Screenshot_from_2024-02-08_04-06-04.png)
            
            ![Screenshot from 2024-02-08 04-05-39.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c449c26a-1935-47bd-809e-51dbfecd9cca/46d2a4e5-b94e-43d3-be51-52a2c30589a2/Screenshot_from_2024-02-08_04-05-39.png)
            
    - To know your wallet address, you can use the following command:
        
        ```
        dfx identity get-wallet --ic
        ```
        
    - Check your cycle balance. **Take a screenshot** showing the cycle balance.
        
        ```
        dfx wallet --ic balance
        ```
        
        ![Screenshot from 2024-02-08 04-05-14.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c449c26a-1935-47bd-809e-51dbfecd9cca/3cf0588e-8ec6-4ff4-9e33-934c9e039da5/Screenshot_from_2024-02-08_04-05-14.png)
        
4. **Deploy your simple Canister to the Internet Computer**:
    - Navigate into a project directory that you created :
        
        ```
        cd bitcoin
        ```
        
    - Deploy your canister to the mainnet:
        
        ```
        dfx deploy -- network ic
        ```
        
    - **Take a screenshot** showing the successful deployment of your canister to the mainnet.
    - Once it deploys successfully then you can check that the cycles have reduced in number.Initially we had 13.898 [TC.Now](http://TC.Now) confirm the balance after deploying on the ic mainnet and calculate  how many cycles you used.

### Submission:

- **Screenshots**: Submit screenshots of the terminal showing
    
    1) The list of identities created and the default one. (Step 2)
    2) The successful transaction of claiming cycles with the faucet coupon. (Step 3)
    3) The successful deployment of your canister to the mainnet.  (Step 4)
    
- **Question 1:** How much cycles do you need for deploying a simple canister to Internet Computer? `Hint: check your balance after the deployment.`
- **Question 2**: What are the implications and importance of using different identities for development and deployment in the Internet Computer ecosystem?