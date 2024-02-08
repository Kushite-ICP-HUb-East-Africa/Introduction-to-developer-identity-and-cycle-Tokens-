# Create a Developer Identity, Claim Cycle Tokens, and Deploy a Simple Canister on IC
This tutorial aims to help you  Create a Developer Identity, Claim Cycle Tokens, and Deploy a Simple Canister on IC.


1. **Apply for Free Cycles from a Cycles Faucet:**
    - Obtain a coupon code for redeeming cycles from a [cycles faucet](https://anv4y-qiaaa-aaaal-qaqxq-cai.ic0.app/). In the survey, enter `0TOICP` as the name of your project. After receiving your coupon, you can then move on to the steps below.
        
      ![Screenshot from 2023-11-27 16-28-43](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/a9a13050-83d7-40da-85dc-11c52bac2607)

        
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
        
       ![Screenshot from 2023-11-27 16-21-04](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/afb30d62-884c-431d-acf9-1014e78e039f)

        
3.  **Claim Cycles with Redeem-Faucet-Coupon and Check Your Balance**:
    - Use the coupon you obtained to redeem your free cycles.
        
        ```
        dfx wallet --ic redeem-faucet-coupon <your coupon-code>
        ```
        
        - This step involves creating a cycles wallet by redeeming free cycles, instead of the usual method of converting ICP tokens.
            
          ![Screenshot from 2023-11-27 16-29-36](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/392fc477-4071-40fd-9f99-82f658656ff3)

            
         ![Screenshot from 2024-02-01 09-00-47](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/e9c2c56a-15b2-4410-ab33-ea7c0e3fc19b)

            
    - To know your wallet address, you can use the following command:
        
        ```
        dfx identity get-wallet --ic
        ```
        
    - Check your cycle balance. **Take a screenshot** showing the cycle balance.
        
        ```
        dfx wallet --ic balance
        ```
        
   ![Screenshot from 2024-02-08 04-05-39](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/4a281f01-3239-4155-bdc7-52d5cbc2dff1)

        
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
    ![Screenshot from 2024-02-08 05-05-41](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/67cb2a01-2498-4309-9f1c-445a747d4dbc)

    - Once it deploys successfully then you can check that the cycles have reduced in number.Initially we had 13.898 [TC.Now](http://TC.Now) confirm the balance after deploying on the ic mainnet and calculate  how many cycles you used.
    ![Screenshot from 2024-02-08 04-03-19](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-developer-identity-and-cycle-Tokens-/assets/81568615/ac307046-2ba6-4b31-b311-d8ab111614ce)


### Submission:

- **Screenshots**: Submit screenshots of the terminal showing
    
    1) The list of identities created and the default one. (Step 2)
    2) The successful transaction of claiming cycles with the faucet coupon. (Step 3)
    3) The successful deployment of your canister to the mainnet.  (Step 4)
    
- **Question 1:** How much cycles do you need for deploying a simple canister to Internet Computer? `Hint: check your balance after the deployment.`
- **Question 2**: What are the implications and importance of using different identities for development and deployment in the Internet Computer ecosystem?