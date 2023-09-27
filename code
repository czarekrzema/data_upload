import gdown
import argparse

file_destinations = {'CICIoT2023','CICIoT2023.zip'}

file_id_dic = {'CICIoT2023','1DPdJb5xXGY5rF1MzfL3EFwDQecH5Od9z'}

def download_file_from_google_drive(id_, destination):
    url = f'https://drive.google.com/uc?id={id_}'
    output = destination
    gdown.download(url, output, quiet=False)
    print(f'{output} download complete!')
    
parser = argparse.ArgumentParser(description = 'data loader for PseudoLab Tutorial Book')

parser.add_argument('--data', type = str, help = 'key for selecting data')

args = parser.parse_args()

download_file_from_google_drive(id_=file_id_dic[args.data], destination=file_destinations[args.data])
