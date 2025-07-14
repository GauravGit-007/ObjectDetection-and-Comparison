# Use official lightweight Python image
FROM python:3.10-slim

# Set working directory inside the container
WORKDIR /app

# Copy everything into the container
COPY . .

# Install required packages
RUN pip install --no-cache-dir ultralytics opencv-python matplotlib pandas notebook nbconvert

# Create output directory if not present
RUN mkdir -p outputs

# Default command: convert notebook to HTML
CMD ["jupyter", "nbconvert", "--to", "html", "task3.ipynb"]
