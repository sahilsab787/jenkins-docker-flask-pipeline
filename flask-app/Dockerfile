FROM python:3.8

# Set working directory
WORKDIR /usr/src/app

# Copy only requirements first
COPY requirements.txt ./

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy rest of the code
COPY . .

# Expose port
EXPOSE 5000

# Run app
CMD ["python", "./app.py"]
