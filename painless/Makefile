all: 
	##################################################
	###                Maplesat                    ###
	##################################################
	+ $(MAKE) -C maplesat

	##################################################
	###                PaInleSS                    ###
	##################################################
	+ $(MAKE) -C painless-src
	cd painless-src && mv painless ../painless

docs:
	rm -rf documents
	doxygen doxygen.config
	mkdir -p documents
	mv html latex documents

clean:
	##################################################
	###                Maplesat                    ###
	##################################################
	+ $(MAKE) -C maplesat clean

	##################################################
	###                PaInleSS                    ###
	##################################################
	+ $(MAKE) clean -C painless-src
	rm -rf painless documents
