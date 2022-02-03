# STEP 1: Install base image. Optimized for Python.
FROM python

# Step 2: Add requirements.txt file
COPY requirements.txt /requirements.txt

# Step 3:  Install required pyhton dependencies from requirements file
RUN pip install -r requirements.txt

# Step 4: Copy source code in the current directory to the container
ADD . /app

# Step 5: Set working directory to previously added app directory
WORKDIR /app

# Step 6: Run App
CMD python manage.py
