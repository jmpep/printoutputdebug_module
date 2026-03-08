# printoutputdebug_module

## requirement
| library | example                               |
|---------|---------------------------------------|
| pprint  | from pprint import pprint |

## usage 
| library                 | example                               |
|-------------------------|---------------------------------------|
| printoutputdebug_module | from printoutputdebug_module import * |

* usage in a class
 create in your class a self variable to get the link to the library
 here "out"

| type | initialisation                                                                                                                                                       |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| in a class | class YouCLASS(Client): <br/>def __init__(self,...,out=None):<br/>self.server=server<br/>self.out=out                                                                |
| in the script | out=outputs(level=args.parameters.level<br/>  ,printout=args.doprint<br/>  ,debugFileName=args.debug_file<br/>,outputFileName=args.output_file<br/>,logFileName=args.log_file) |

| Example of usage                                                                          |
|---------------------------------------------------------------------------------------------------------|
| #here for DEBUG level<br/>self.out.DEBUG<br/>self.out.echo(self.out.DEBUG,'YOUR MESSAGE')               |
| out.writeOutput('w',"<your message>")                                                                   | 
| #use humanJsonFormat to show JSON in a human format<br/>out.echo(DEBUG,out.humanJsonFormat(configslist)) |