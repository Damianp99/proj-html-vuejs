<template>
  <div id="posts">
    <div class="container">
      <div class="row">
        <div class="col-4">
          <h5 class="fw-bolder small">POPULAR POSTS</h5>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-55.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                simple ways to have a pretty face
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-56.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                ranking the greatest players in basketball
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-57.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                4 ways to look cool in glasses
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-58.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                top camper trailer towing tips
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-59.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                5 lovely walks in new york
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
        </div>
        <div class="col-4">
          <h5 class="fw-bolder small">RECENT POSTS</h5>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-65.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                main reason to stop texting and driving
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-66.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                tips to help you quickly prepare your lunch
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-67.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                why should i buy a smartwatch?
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-68.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                the best augmented reality smartglasses
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
          <div class="d-flex flew-wrap post-border pt-2">
            <img
              class="post-img me-2"
              src="../assets/images/blog-69.jpg"
              alt="post picture"
            />
            <div class="d-flex flex-column">
              <h6 class="text-capitalize fw-normal">
                12 healthiest foods to eat for breakfast
              </h6>
              <div><span class="text-muted small">January 12, 2019</span></div>
            </div>
          </div>
        </div>
        <div class="col-4">
          <h5 class="fw-bolder small">FEATURED POSTS</h5>
          <div>
            <button class="btn btn-blue">RECIPES</button>
            <h5 class="text-capitalize">
              tips to help you quickly prepare your lunch
            </h5>
          </div>
          <div>
            <h5 class="fw-bolder small">FEATURED AUTHOR</h5>
            <div class="d-flex flew-wrap pt-2">
              <img
                class="post-img me-2 avatar"
                src="../assets/images/avatar.jpg"
                alt="post picture"
              />
              <div class="d-flex flex-column">
                <h6 class="fw-bolder">John Doe</h6>
                <div>
                  <span class="text-muted small"
                    >Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Posts",
};
</script>

<style lang="scss" scoped>
.post-border {
  padding-bottom: 10px;
  border-top: 0px;
  border-left: 0px;
  border-right: 0px;
  border-bottom: 1px solid lightgray;
  border-style: dotted;
}
.post-img {
  height: 50px;
  width: 50px;
}
.avatar {
  height: 100px;
  width: 100px;
}
</style>