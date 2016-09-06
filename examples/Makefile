JL_SHARE = $(shell julia -e 'print(joinpath(JULIA_HOME,Base.DATAROOTDIR,"julia"))')
JL_CONFIG := $(JL_SHARE)/julia-config.jl
CFLAGS   += $(shell $(JL_CONFIG) --cflags)
CXXFLAGS += $(shell $(JL_CONFIG) --cflags)
LDFLAGS  += $(shell $(JL_CONFIG) --ldflags)
LDLIBS   += $(shell $(JL_CONFIG) --ldlibs)

LDFLAGS += -L/home/tracy/prj/julia/julia-7df91d34e9/lib/julia
LDLIBS += -lm -Wl,-rpath,/home/tracy/prj/julia/julia-7df91d34e9/lib/julia

all: embedding
