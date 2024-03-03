The Web3 Company, where I did my previous internship was RariKo - a web3-based social media platform for building communities. 
During my internship tenure at RariKo, I was assigned to implement/work on 3 features. 
a. Implement a referral system - for both Windows and mobile interfaces.
b. Implement wagmi payments feature - for both Windows and mobile interfaces. 
c. Add new features to Community Section - 
    i. Allowing Admin only to update the community details - Name, Description, Tags, Profile Picture. 
    ii. Redesigning Components - Had to re-design some components to make the feature loosely coupled and highly cohesive architecture
    iii. Added custom role feature - Allowing admins to create a custom role, which can be normal or token-based, and assign it to the community members. Along with that added a feature to assign an admin role to any member of the community.

Diving deep into the features - 
a. Referal System: 
I developed the referral system using Node.js backend and integrated it into the frontend using React.js and Material UI. To refer a user, there are two options available: ​
    1. Referral Link: A unique referral link is automatically generated when a new user is created. The user can share this link with others, allowing them to sign up using the link.​​
    2. Whitelisting Contract Addresses: An existing user can whitelist the web3 contract address of a new user. Once the whitelisting is successful, the new user can sign up.​​

New users can only sign up using a referral link or a whitelisted web3 contract address. ​​​
When a new user signs up through a referral link or whitelisting, the person who provided the referral link or did the whitelisting receives a reward of 1000 XP points.​​​
Users can keep track of how many people they have whitelisted and how many people have used their referral link to sign up.​

b. Wagmi Payments:
I designed and coded the UI for wagmi payments features. This includes developing a form-like component. 
A user-based story to the feature: 
a. The client first has to search for the user it has to send the crypto to. As the user types in the search bar, the list of users matching the search query is displayed after being fetched from the backend. To optimise it, I implemented a debounce function to reduce the number of API calls.
b. Once the user is selected, the client has to choose the token type - Polygon or Ethereum or Binance Smart Chain.
c. After that it has to choose the address of the user to whom it has to send the crypto. The address is fetched from the backend simultaneously after the client has selected the user to whom the crypto has to be sent.
d. Then the client has to choose the token type - USDC or USDT or MATIC
e. Then the client enters the amount and clicks on the send button.

All the transactions are displayed below this form component in the form of a table. 

I also developed its backend logic and a few other controller functions such as retrieval of contract addresses, etc. ​
During this, I also got a chance to work on a few web3 JavaScript libraries.​​
I collaborated with one of my colleagues who was responsible for developing the rest of the features including heavy knowledge and familiarity with web3 frameworks.​​

c. Community Section:
i. Updating Community Details: I have added a new feature that enables the admin(s) of a specific community to update the details of the community including profile pic, community title, description etc. ​
ii. Customized Roles: Community admin(s) have exclusive privileges to create new roles and assign or remove them from community members, including admin roles. Community roles can be normal or token gated.​
iii. Redesigning Components: I had to re-design some components to make the feature loosely coupled and highly cohesive architecture.​

For normal roles, the admin only needs to enter the role name, and a new role will be created automatically. The ID of the role is dependent on the number of roles already present within that particular community. However, for token-gated communities, the admin must select the token address of an NFT/Token, the minimum cryptocurrency required to hold that role, the role name, and the token symbol. I developed the backend and frontend to meet the specified requirements.​ 