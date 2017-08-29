# ComRouter

**platform**： Ios Swift3

ComRouter is a componentized intermediate router, ComRouter is a component of the middle of the router, call the external interface between the various components

## usage

> Direct call

	ComRouter.shareInstance.call("ComRouteCompenontTest", "ComRouteInterface", "comRouteForParams").params("one", "two", paramNames: ["test","string"]) { (result,error) in
            print(error as Any)
    }
    
    
> Chain call

	ComRouter.shareInstance.moduleName("ComRouteCompenontTest").className("ComRouteInterface").funcName("comRouteForParams").params("one", "two") { (result,error) in
            print(error as Any)
    }
