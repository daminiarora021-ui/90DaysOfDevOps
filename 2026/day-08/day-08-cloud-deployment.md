## Part 1: Launch Cloud Instance & SSH Access (15 minutes)

**Step 1: Create a Cloud Instance**

screenshot :
![1](images/1.jpg)


**Step 2: Connect via SSH**


screenshot :
![2](images/2.jpg)


### Part 2: Install Docker & Nginx (20 minutes)

**Step 1: Update System**
sudo apt update 

screenshot :
![3](images/3.jpg)

**Step 3: Install Nginx**

sudo apt install nginx

**Verify Nginx is running:**

systemslt status nginx


screenshot :
![5](images/5.jpg)





### Part 3: Security Group Configuration (10 minutes)

**Test Web Access:**
Open browser and visit: `http://<your-instance-ip>`

You should see the **Nginx welcome page**!

📸 **Screenshot this page** - you'll need it for submission


