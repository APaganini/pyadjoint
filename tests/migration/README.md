Currently working tests:

- [x] assembled_action
- [x] burgers_newton
- [x] burgers_newton_time_functional
- [x] burgers_oo
- [x] burgers_picard
- [x] cahn_hilliard
- [ ] changing_vector (replay_dolfin is not implemented)
- [ ] checkpoint_burgers (checkpointing is not implemented)
- [ ] checkpoint_burgers_newton (checkpointing is not implemented)
- [ ] checkpoint_online (checkpointing is not implemented)
- [ ] checkpoint_stokes (checkpointing is not implemented)
- [ ] compute_tlm_list_parameter (compute_tlm is not implemented. It is possible to get tlm values, but it involves interacting with tape and block outputs directly)
- [x] curl-curl
- [x] default_parameters
- [x] differentiability-dg-upwind
- [x] differentiability-stokes
- [x] distributed_control
- [ ] dolfin_adjoint_variable (pyadjoint does not have DolfinAdjointVariable)
- [ ] expression_derivative (The design of the expression breaks how pyadjoint stores the expression checkpoints - this issue needs to be discussed further)
- [x] expression_derivative_cpp 
- [x] expression_derivative_inline_cpp
- [ ] expression_updates (replay_dolfin is not implemented)
- [x] facet_integrals
- [x] fg_constant
- [x] fg_constants
- [ ] function_assign_lincom (Assign linear combination not implemented)
- [ ] function_assigner (FunctionAssigner not implemented)
- [ ] function_assigner_givsub (FunctionAssigner not implemented)
- [ ] functional_dependencies (Invalid - adjointer/Functional not present. Might be valid if rewritten)
- [ ] functional_form (invalid - pyadjoint doesnt have Functional)
- [ ] functional_operations (certain AdjFloat operations doesnt have TLM/Hessian support)
- [x] functional_value
- [ ] gst_mass (compute_gst not implemented)
- [x] heat
- [ ] hessian_callback (Hessian callback not implemented)
- [ ] hessian_eps (Eigendecomposition of Hessian not implemented)
- [x] hessian_identity
- [ ] hessian_identity_list (Should work but testing interface is lacking for hessian with multiple controls)
- [ ] hessian_identity_list2 (Should work but testing interface is lacking for hessian with multiple controls)
- [ ] interpolate (Interpolate is not implemented yet)
- [ ] krylov_reevaluate (KrylovSolver is not implemented)
- [ ] linear_solver (LinearSolver is not implemented)
- [x] list_parameter 
- [ ] localsolver (LocalSolver not implemented)
- [ ] localsolver_factorize (LocalSolver not implemented)
- [ ] lusolver_changing (replay_dolfin not implemented)
- [ ] lusolver_reassemble (replay_dolfin not implemented)
- [x] lvs
- [ ] manual_hessian (Might not be relevant as Hessian is already implemented)
- [ ] matrix_free_burgers (KrylovSolver is not implemented)
- [ ] matrix_free_heat (KrylovSolver is not implemented)
- [ ] matrix_free_simple (KrylovSolver is not implemented)
- [ ] matrix_summation (Matrix summation is not implemented)
- [ ] mpec (compute_tlm is not implemented. It is possible to get tlm values, but it involves interacting with tape and block outputs directly)
- [ ] multimesh_poisson (multimesh is not implemented)
- [ ] navier_stokes (Seems backend.derivative(form, c, dc) does not accept dc to be Sum instance? Projecting tlm_input makes this work with Hessian)
- [x] newton_constant 
- [x] noannotations
- [ ] nullspace (KrylovSolver is not implemented)
- [ ] nullspace_linear_solver (LinearSolver is not implemented)
- [x] nvs
- [ ] ode_fitzhughnagumo (PointIntegralSolver is not implemented)
- [ ] ode_solver (PointIntegralSolver is not implemented)
- [ ] ode_tentusscher (PointIntegralSolver is not implemented)
- [ ] ode_tentusscher_quick (PointIntegralSolver is not implemented)
- [ ] ode_vector (PointIntegralSolver is not implemented)
- [x] optimal_control_bfgs
- [x] optimal_control_mms
- [ ] optimization_checkpointing (optimization is not implemented)
- [ ] optimization_moola (optimization is not implemented)
- [ ] optimization_optizelle (optimization is not implemented)
- [ ] optimization_optizelle_algebra (optimization is not implemented)
- [x] optimization_pyipopt
- [ ] optimization_pyopt (optimization is not implemented)
- [x] optimization_scalar
- [x] optimization_scipy
- [ ] optimization_tao (TaoSolver is not implemented, maybe it should live in fenics_adjoint?)
- [ ] periodic (PeriodicBC is not implemented)
- [ ] petsckrylov_reevaluate (PETScKrylovSolver is not implemented)
- [x] picard-linearisation
- [x] pointwise_functional
- [ ] pointwise_functional_one_point (PointwiseFunctional does not exist in pyadjoint)
- [ ] pointwise_functional_regularisation (PointwiseFunctional does not exist in pyadjoint)
- [ ] pointwise_functional_two_points (PointwiseFunctional does not exist in pyadjoint)
- [ ] pointwise_functional_vector (PointwiseFunctional does not exist in pyadjoint)
- [ ] preassembly_efficiency (assemble kwarg "cache" is not implemented)
- [x] projection
- [x] reduced_functional (ReducedFunctional.hessian is not implemented)
- [ ] reduced_functional_cache (ReducedFunctional kwarg cache is not implemented)
- [x] reduced_functional_constants
- [x] reduced_functional_evaluation
- [ ] rush_larsen (PointIntegralSolver is not implemented)
- [x] shallow_water 
- [x] shallow_water_time_functional
- [x] split
- [x] stokes
- [ ] stokes_krylov (KrylovSolver is not implemented)
- [ ] stokes_maday (Optimization is not implemented)
- [ ] stokes_petsckrylov (PETScKrylovSolver is not implemented)
- [x] supg
- [ ] svd_bc_simple (compute_gst is not implemented)
- [ ] svd_burgers (compute_gst is not implemented)
- [ ] svd_burgers_perturb (compute_gst is not implemented)
- [ ] svd_simple (compute_gst is not implemented)
- [x] taylor_hessian 
- [x] time_dependent_data
- [ ] time_functionals (invalid - pyadjoint doesn't have functional)
- [x] time_functionals_no_annotation
- [ ] timeforms (invalid - pyadjoint doesn't have timeforms)
- [ ] tlm_burgers (compute_gradient_tlm is not implemented)
- [ ] tlm_list_parameter (compute_gradient_tlm is not implemented)
- [ ] tlm_scalar_parameter (compute_gradient_tlm is not implemented)
- [ ] tlm_simple (compute_gradient_tlm is not implemented)
- [x] upwind
- [x] viscoelasticity
- [ ] zero_derivative (How pyadjoint should handle zero derivatives is yet to be decided)