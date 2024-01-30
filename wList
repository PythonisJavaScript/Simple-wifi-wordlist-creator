import sys

def creWoList( **ka ):

	redColor = "\033[1;31m"

	greenColor = "\033[1;32m"

	name = ka[ "combinationName" ].strip()

	fName = ka[ "fileName" ].strip()

	try:

		digiLen = int( ka[ "digitsLength" ] )

	except:

		print( f"\n{ redColor }Insert the data correctly!\n" )

		sys.exit( 0 )

	if name == None or name == "" or digiLen == None or fName == "" or fName == None:

		print( f"\n{ redColor }Insert the data correctly!\n" )

		sys.exit( 0 )

	try:

		f = open( f'{ fName }.txt', "x" )

		numLen = "{:%s}" % f'0{ digiLen }d'

		for x in range( 0, 10**100 ):

			if len( str( x ) ) == int( digiLen ) + 1:

				break

			f.write( f"\n{ name }{ numLen.format( x ) }" )

		f.close()

		print( f"\n{ greenColor }The file has been successfully created!\n" )

	except:

		print( f"\n{ redColor }The file name is existed!\n" )



creWoList( fileName = str( input( "Create file name : " ) ) , combinationName = str( input( "Combination name : " ) ), digitsLength = str( input( "Digits length : " ) ) )
