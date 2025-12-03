I created one VPC with a CIDR range to build a private network.
Inside this VPC, I created two public subnets and two private subnets by dividing the IP range. The public subnets were connected to the internet using an Internet Gateway.
The private subnets were isolated but got outbound internet access through a NAT Gateway placed in one public subnet.
I launched a Free Tier EC2 instance inside my public subnet and assigned it a public IP so it can be accessed from the internet.
After connecting via SSH, I installed Nginx and placed my resume HTML file.
Cost monitoring is important because new users often forget to stop or delete resources that keep charging in the background.
Sudden bill increases usually happen when EC2, NAT Gateways, Load Balancers, or large S3 storage are left running accidentally.
