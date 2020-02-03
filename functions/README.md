After installing MNE, attempt to import raw EEG in .cnt files by:

	import mne
	file = mne.io.read_raw_cnt("files.cnt")
	print(file.info)
	eeg = file.get_data()
	
If errors return "CNTEventype has no latency", then:

	cd python3.7/site-packages/mne/io/cnt
	vi cnt.py
	
	Comment line 428 to 431, you will get same result 
	rsync -auxv nedc_tuh_eeg@www.isip.piconepress.com:~/data/tuh_eeg_abnormal .
