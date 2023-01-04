# Docker-Notes

           ┌──────────────┐
           │  Docker CLI  │ ◄────────────  Command Line Insterface for users
           └───────┬──────┘
                   │
                   │
                   │
                   │
           ┌───────┴───────┐
           │ Docker daemon │◄───────────── Provides API Services and other docker management services
           └───────┬───────┘
                   │
                   │
                   │
          ┌────────┴──────┐
          │  Container-D  │◄──────────────Container life cycle managment service
          └──────────┬────┘
                     │
         ┌───────────┼─────────── - - -
         │           │
   ┌─────┤        ┌──┴─┐
   │ shim│        │Shim│
   ├─────┤        ├────┤
   │ runc│        │runc│◄────────────────────Reference implimentation of OCI Specification
   └──┬──┘        └──┬─┘
      │              │
┌─────┴─────┐   ┌────┴──────┐
│ Container │   │ Container │
│  Instance │   │ Instance  │◄───────────────   Runtime instances of container-images
└───────────┘   └───────────┘


The above diagram outlines the Docker Architecture.
