
### Commands

export GOOGLE_APPLICATION_CREDENTIALS="../wired-glider-441301-e1-b6a080d0f979.json"
python3 preprocess.py
python3 train.py --dataset_path=./processed_data/tokenized_amazon_reviews --output_dir=./distilbert-sentiment-model
python create_test_dataset.py
python test.py