After installing MNE, attempt to import raw EEG in .cnt files by:

	'''python3
	import mne
	file = mne.io.read_raw_cnt("files.cnt")
	print(file.info)
	eeg = file.get_data()
	'''
