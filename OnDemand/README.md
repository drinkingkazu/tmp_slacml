# Set up SLAC computing environment

Please read and follow the below steps as soon as you can so that we can ensure that we run into minimal issues on the day of the classes. If you have any problems, feel free to email Yee at ytl@slac.stanford.edu or to contact us on the SLAC #ml-class Slack channel.

## Accounts and Access
Many of you already have SLAC UNIX accounts, however, the SDF will be using SLAC Windows accounts. This is in accordance to a long term goal to simplify our operational infrastructure and reduce the technical debt that we have accumulated.
If you do not already have a SLAC Windows account, you can create one if you already have a UNIX account by visiting http://ad-account.slac.stanford.edu/. Note that you will need to have your SLAC training up-to-date.

## Getting started

### 1. Login
* Goto https://ondemand-dev.slac.stanford.edu in your favorite web browser. You are more than welcome to browse the documentation.
* Click on the "Login" button
* You will be presented with a CILogin screen: This allows us to provide delegated authentication so that you may log on with non-SLAC credentials. As with all good things, you'll have to wait for this feature to be implemented.
* Select **SLAC National Accelerator Laboratory** from the drop down list.
* The standard SLAC single-sign-on-page will be presented: enter your SLAC Windows credentials. You may also be asked for your '2-factor' key using Duo.
* You should be presented with the 'ondemand' frontend.
### 2. Launch jupyter
- at the top of the 'ondemand' webpage that we just logged into, click on 'Interactive Apps'
- Select 'Jupyter' from the list
- You should be presented with a set of options to launch a Jupyter instance
- Select 
  - Jupyter Instance: blah
  - leave "Use JupyterLab" unchecked
  - Partition: ml
  - Number of hours: 4
  - Number of CPU cores: 4
  - Total Memory to allocate: 12228
  - Number of GPUs: 1
  - GPU Type: Any
- Click on the big blue 'Launch' button at the bottom

### 3. Wait

- After a few moments, the webpage should update with a 'Connect to Jupyter Instance' button - clicking on this will bring up a Jupyter window

### 4. Party
3. Execute a simple command in the cell
    ```
    import torch
    torch.Tensor([0.]).cuda()
    ```
