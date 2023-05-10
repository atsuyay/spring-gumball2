# CMPE 172 - Lab #10 - DevOps CI/CD Notes

## CI Workflow (Spring Gumball) 

![CI Java CI with Gradle](images/CI_build.PNG) Figure 1. Shows successful workflow of Java CI with Gradle

## CD Workflow (Spring Gumball) 

![CD GKE Service Account](images/gke_service_account.PNG) Figure 2. Shows created GCP Service Accoucnt

![CD GKE Service Account JSON Key](images/gke_json_key.PNG) Figure 3. Shows generated JSON Service Account Key

![CD GKE GitHub Secrets](images/gke_json_key.PNG) Figure 4. Shows GitHub repository secrets

![CD GKE Release](images/CD_release.PNG) Figure 5. Shows new release which will trigger CD workflow.

![CD GKE Building Workflow](images/CD_building_workflow.PNG) Figure 6. Shows CD workflow building.

![CD GKE Workflow Built](images/CI_build.PNG) Figure 7. Shows successful CD workflow build.

![CD GKE All Workflows](images/Github_actions_workflows.PNG) Figure 8. Shows all GitHub actions workflows.

![GKE Cluster](images/gke_cluster.PNG) Figure 9. Shows GKE Cluster named "cmpe172-lab10"

![GKE Workload](images/gke_workload.PNG) Figure 10. Shows GKE spring-gumball-deployment with 2 pod running.

![GKE Service](images/gke_service.PNG) Figure 11. Shows GKE service called spring-gumball-service running on Node Port.

![GKE Ingress](images/gke_ingress.PNG) Figure 12. Shows spring-gumball-lb running on IP 34.117.90.182 which can be access by anyone.

![GKE Spring Gumball Web Page](images/spring-gumball-website.PNG) Figure 13. Shows spring-gumball web page running on 34.117.90.182.


### Challenges Encountered
I had challenges with gke-credentials and have to give permission when creating the GKE Service Account as my CD builds were failing before giving permissions.
