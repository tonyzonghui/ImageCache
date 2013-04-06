## ImageCache

##### A basic image cache system for storing images in memory and on disk

Usage: 

	+ (ImageCache *)sharedImageCache;
	
	- (UIImage *)imageForKey:(NSString *)key;
	
	- (BOOL)hasImageWithKey:(NSString *)key;
	
	- (void)storeImage:(UIImage *)image withKey:(NSString *)key;
	
	- (BOOL)imageExistsInMemory:(NSString *)key;
	
	- (BOOL)imageExistsInDisk:(NSString *)key;
	
	- (NSUInteger)countImagesInMemory;
	
	- (NSUInteger)countImagesInDisk;
	
	- (void)removeImageWithKey:(NSString *)key;
	
	- (void)removeAllImages;
	
	- (void)removeAllImagesInMemory;
	
	- (void)removeOldImages;
	
##### Use with cocoapods

	pod 'ImageCache', '~>0.0.1'